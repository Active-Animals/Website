WIP

<div id="bp_quick_jump"></div>

<script type="text/javascript">
    var BP_ontology_id = "ENVO";</script>

<script src="https://code.jquery.com/jquery-migrate-1.2.1.min.js"></script>
<script src="https://bioportal.bioontology.org/javascripts/plugins/jquery.bioportal_autocomplete.js"></script>
<script src="https://bioportal.bioontology.org/javascripts/widgets/quick_jump.js"></script>

<script type="text/javascript">
jQuery(function($){
    var input = $('#bp_quick_jump input');

    function attachAutocomplete() {
        input.off('bioportal_autocomplete_select');
        input.on('bioportal_autocomplete_select', function(e, data){
            if(data && data.ontology && data.conceptId){
                var url = 'https://bioportal.bioontology.org/ontologies/' +
                          encodeURIComponent(data.ontology) +
                          '/?p=terms&conceptid=' +
                          encodeURIComponent(data.conceptId);
                window.open(url, '_blank');
            }

            // Clear input for next search
            setTimeout(function(){
                input.val('');
                attachAutocomplete();
            }, 50);
        });
    }

    attachAutocomplete();
});
</script>
