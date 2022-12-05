---
layout: default
title: JavaScript
---

<script>
btn1.addEventListener("click", makeSentence);
function makeSentence() {

var person = {
    names: [ "Bruno", "B", "Fiona", "Freddy", "Mini", "Marvin", "Alice", "Bob", "Jane", "Arthur", "Vincent", "Amy", "He", "She" ],
    verbs: [ "speaks", "eats", "runs", "walks", "drinks" ],
    adverbs: ["slowly", "quickly", "nicely", "noisily", "a lot", "a little", "rarely" ]
   
};
  
var i;
var text = "";
for (i = 0; i < person.names.length; i++) {

  name = person.names[i];
  verb = person.verbs[Math.floor(Math.random() * person.verbs.length)];
  adv = person.adverbs[Math.floor(Math.random() * person.adverbs.length)]; 
  text += name + " " + verb + " " + adv + "<br>";
  document.getElementById("demo").innerHTML = text;
 }  
}
</script>****
