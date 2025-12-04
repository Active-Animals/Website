WIP

<div id="bp_quick_jump"></div>

<script type="text/javascript">
    var BP_ontology_id = "ENVO";
</script>

<script src="https://code.jquery.com/jquery-1.11.2.min.js"></script>
<script src="https://code.jquery.com/jquery-migrate-1.2.1.min.js"></script>
<script src="https://bioportal.bioontology.org/javascripts/plugins/jquery.bioportal_autocomplete.js"></script>
<script src="quick_jump.js" type="text/javascript" charset="utf-8"></script>

<script type="text/javascript">
jQuery(function($){
    var input = $('#bp_quick_jump input');

    function attachAutocomplete() {
        input.off('bioportal_autocomplete_select'); // remove previous handler
        input.on('bioportal_autocomplete_select', function(e, data){
            if(data && data.ontology && data.conceptId){
                var url = 'https://bioportal.bioontology.org/ontologies/' 
                          + encodeURIComponent(data.ontology) 
                          + '/?p=terms&conceptid=' 
                          + encodeURIComponent(data.conceptId);

                // Create a temporary <a> element for proper browser behavior
                var link = document.createElement('a');
                link.href = url;
                link.target = '_blank';
                link.rel = 'noopener noreferrer';
                link.click(); // triggers standard link behavior
            }

            setTimeout(function(){
                input.val('');
                attachAutocomplete(); // re-attach handler
            }, 50);
        });
    }

    attachAutocomplete();
});
</script>
