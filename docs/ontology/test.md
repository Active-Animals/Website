WIP

<div id="bp_quick_jump"></div>

<script type="text/javascript">
    var BP_ontology_id = "ENVO";
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


// Second item

<input id="envo_search" placeholder="Search ENVO branch...">

<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="https://code.jquery.com/ui/1.13.2/jquery-ui.min.js"></script>

<script>
const API_KEY = "96ba3d84-e3d8-45bc-99cb-2810d15eed4d";
$("#envo_search").autocomplete({
    minLength: 2,
    source: async function(req, res){
        let r = await fetch(
          "https://data.bioontology.org/search?q=" +
          encodeURIComponent(req.term) +
          "&ontology=ENVO&root=ENVO:01000060",
          { headers: { "Authorization": "apikey token=" + API_KEY } }
        );
        let j = await r.json();
        res(j.collection.map(x => ({ label: x.prefLabel, iri: x['@id'], ont: x.links.ontology })));
    },
    select: function(e, ui){
        let url = "https://bioportal.bioontology.org/ontologies/ENVO/?p=terms&conceptid=" + encodeURIComponent(ui.iri);
        window.open(url, "_blank");
    }
});
</script>
