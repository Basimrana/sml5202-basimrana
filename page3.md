<h1>Homework 3</h1>

<p>
<img src="https://www.tanzania-expeditions.com/wp-content/uploads/2014/05/africa-wildlife-giraffes-trees-sky-photo.jpg" style="width:170px;height:170px;margin-right:15px;float:left;" >
  ssssssssssss and This is a giraffe ggggggggggggggggggggggggggggg
</p>

<div style="clear:both;"></div>

<h2>My First JavaScript</h2>
<button onclick="makeSentence()">Click me</button>

<p id="demo"></p>

<script>
function makeSentence() {

var person = {
names: [ "Basim", "Rana", "Naseer", "Marvin", "Sam" ],
verbs: [ "speaks", "eats", "runs", "walks", "drinks" ],
adverbs: ["slowly", "quickly", "nicely", "noisily", "a lot" ]

};

var i;
var text = "";
for (i = 0; i < person.names.length; i++) {

name = person.names[i];
verb = person.verbs[Math.floor(Math.random() * person.verbs.length)];
adv = person.adverbs[Math.floor(Math.random() * person.adverbs.length)];

text +=name + " " + verb + " " + adv + "<br>";

document.getElementById("demo").innerHTML = text;
}


}

</script>

<style>
* {
  box-sizing: border-box;
}

/* Create two equal columns that floats next to each other */

.column {
  float: left;
  width: 50%;
  padding: 10px;
}

/* Border around the container */

.row {
   border: 1px solid black;
}

/* Clear floats after the columns */

.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Responsive layout - makes the two columns stack on top of each other instead of next to each other */

@media screen and (max-width: 600px) {
  .column {
    width: 100%;
  }
}
</style>

<div class="row">
  <div class="column">
    <h2>Column 1</h2>
    <p><img src="https://www.tanzania-expeditions.com/wp-content/uploads/2014/05/africa-wildlife-giraffes-trees-sky-photo.jpg" /></p>
  </div>
  <div class="column">
    <h2>Column 2</h2>
    <p>The West African giraffe (G. c. peralta) is endemic to south-western Niger.[24] This animal has a lighter pelage than other subspecies,[40]:322 with red lobe-shaped blotches that reach below the hocks. The ossicones are more erect than in other subspecies and males have well-developed median lumps.[33]:52–53 It is the most endangered subspecies within Giraffa, with 400 individuals remaining in the wild.[24] Giraffes in Cameroon were formerly believed to belong to this species, but are actually G. c. antiquorum.[32] This error resulted in some confusion over its status in zoos, but in 2007, it was established that all "G. c. peralta" kept in European zoos actually are G. c. antiquorum. The same 2007 study found that The West African giraffe was more closely related to the Rothschild's giraffe than the Kordofan and its ancestor may have migrated from eastern to northern Africa and then to its current range with the development of the Sahara Desert. At its largest, Lake Chad may have acted as a barrier between West African and Kordofan giraffes during the Holocene (before 5000 BC).[32]</p>
  </div>
</div>
