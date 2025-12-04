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
        if (input.data('ui-autocomplete')) {
            input.autocomplete('destroy');
        }

        input.bioportal_autocomplete({
            ontology: BP_ontology_id,
            select: function(event, ui){
                if(ui.item && ui.item.ontology && ui.item.conceptId){
                    var url = 'https://bioportal.bioontology.org/ontologies/' +
                              encodeURIComponent(ui.item.ontology) +
                              '/?p=terms&conceptid=' +
                              encodeURIComponent(ui.item.conceptId);
                    window.open(url, '_blank');
                    input.val('');
                    return false;
                }
            }
        });
    }

    attachAutocomplete();
});
</script>

