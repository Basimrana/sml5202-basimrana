<h1>Random Idiom using JSON</h1>

<button type="button" class="new-quote button">Show Idiom</button>
<dl id="quote"></dl>

<script>
const endpoint = 'https://basimrana.github.io/sml5202-basimrana/dataset/idioms.json';

function getQuote() {
fetch(endpoint)
.then(function (response) {
return response.json();
})
.then(function(data){
let id = Math.floor(Math.random() * 6);
let idiom = (data.idioms[id].idiom);
let meaning = (data.idioms[id].meaning);
let example = (data.idioms[id].example);

document.querySelector('#quote').innerHTML = "<dt>" + idiom + "</dt>" + "<dd><strong>Example:</strong> " + example + "</dd><dd><strong>Meaning:</strong> " + meaning + "</dd>";

//console.log(data.idioms[id].idiom)
})
.catch(function () {
console.log("Error occured");
});
}

const newQuoteButton = document.querySelector('.new-quote');
newQuoteButton.addEventListener('click', getQuote);

</script>
