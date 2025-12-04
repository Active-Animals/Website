WIP

<div id="bp_quick_jump" data-apikey="96ba3d84-e3d8-45bc-99cb-2810d15eed4d"></div>

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
        input.off('bioportal_autocomplete_select');

        input.on('bioportal_autocomplete_select', function(e, data){
            if(data && data.ontology && data.conceptId){
                var url = 'https://bioportal.bioontology.org/ontologies/' +
                          encodeURIComponent(data.ontology) +
                          '/?p=terms&conceptid=' +
                          encodeURIComponent(data.conceptId);
                window.open(url, '_blank');
            }

            setTimeout(function(){
                input.val('');
                attachAutocomplete();
            }, 50);
        });

        // Also capture clicks on the autocomplete menu items directly
        $(document).on('click', '.ui-menu-item', function(){
            var item = $(this).data('ui-autocomplete-item');
            if(item && item.ontology && item.conceptId){
                var url = 'https://bioportal.bioontology.org/ontologies/' +
                          encodeURIComponent(item.ontology) +
                          '/?p=terms&conceptid=' +
                          encodeURIComponent(item.conceptId);
                window.open(url, '_blank');
                input.val('');
            }
        });
    }

    attachAutocomplete();
});
</script>
