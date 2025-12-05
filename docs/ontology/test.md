WIP

<div id="bp_quick_jump"></div>

<script type="text/javascript">
    var BP_ontology_id = "ENVO";
    var BP_search_branch = "http://purl.obolibrary.org/obo/ENVO_01000060";
</script>

<script src="https://code.jquery.com/jquery-1.11.2.min.js">
</script>

<script src="https://bioportal.bioontology.org/javascripts/widgets/quick_jump.js">
</script>

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


<div style="width: 100%; height: 500px;">
    <iframe 
        frameborder="0" 
        src="https://bioportal.bioontology.org/widgets/visualization?ontology=ENVO&class=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FENVO_01000060&apikey=96ba3d84-e3d8-45bc-99cb-2810d15eed4d" 
        style="width: 100%; height: 100%; display: block;">
    </iframe>
</div>

<iframe 
    frameborder="0" 
    src="https://bioportal.bioontology.org/widgets/visualization?ontology=ENVO&class=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FENVO_01000060&apikey=96ba3d84-e3d8-45bc-99cb-2810d15eed4d">
    style="width: 800px; height: 800px; display: block;">
</iframe>
