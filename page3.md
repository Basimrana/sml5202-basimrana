<h1>Homework 3</h1>

<p>
<img src="https://www.tanzania-expeditions.com/wp-content/uploads/2014/05/africa-wildlife-giraffes-trees-sky-photo.jpg" style="width:70%;">
  This is a giraffe. ssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssss
</p>


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
