---
title: Shrine of Luck
layout: local
order: 3
---
<div class="w3-half">
<h2>Description</h2>
  <ul>
<li>You walk past the StoneHill Inn heading towards the minners trail and on he right you see the shrine. 
It appears to be made of stone from the surronding ruins around town.</li>
    <li>Through the window you see a young elf working at the alter. Whe she turns you notice her injuries. 
Her left arm is in a cloth sling and there are various stages of brusing on her face.</li>
    <li>You enter the Shrine and the elf immeditaley looks up quickly taking in your apperance. "You must be the travelers I have heard so much about.
      How can I help you?</li>
  </ul>
</div>
<div class="w3-half">
<h2>People</h2>
<p>Sister Garaele</p>
  <button id="speak"> Speak </button>
  <p id="said"></p>
  <button id="next">Next</button>
  <div id="extra">
    <button id="conyberry" class="w3-button w3-round w3-lime"><a href="travel.html">Conyberry and Agathas Lair</a></button>
  </div>
</div>
<script>
  $("document").ready(function(){
    $("#speak").click(function(){
      let first = "She leads you past the shrine and into the back hall it has a curain seperating it from the main room and upon entering you notice that it is crammed packed with relics and other objects with a small walking path leading to a door. When opened the door leads to a small yard. Chickens are running around trying to catch worms and other bugs that live in the grass. Her home is a small cottage tucked into the corner of the yard. She welcomes you in to a small room with a open door way straight ahead and a closed door on the right. She invites you to sit at the chairs around the table to the left.'Welcome to my home. Please take a seat while I put water on for tea. Oh my name is Sister Garaele'. She walkes through the open door way and there is the clear sound of water being put into a kettel and rummaging in a cuppord."
      $("#said").html(first)
    });
  });
</script>
<script> 
  let count = 0;
      const conversation = [
        {key: 1, 
         quote: "She enters the room bringing tea in to you with a plate of biscuts and jam. 'So I hear that you are travelers that have saved Sildar Hallwinter,and saved the captives from the redbrand hideout.'"
        }, {
          key: 2, 
          quote: "I am a part of a rather secerative group called the Harpers we advocating for equality and oppose the abuse of power and protect the weak the poor and the oppresed. I am hoping to get rid of the redbrands all together in Phanalin but for now I must continue my orders."
        }, {
         key: 3, 
         quote: "You might notice that I am a littel under the weather. I was given the task of tracking down a banshee named Agatha to get information on a spellbook for my superiors." 
        }, {
          key: 4, 
          quote: "She is supposed to persuade a Banshee named Agatha to answer a question about a spell book. We need to know the books location and also any information regaurding its owner Bowgentle. Acoording to rumor Agatha will appear to only those that she deems worthy and who bring a gift that pleases her. Unfortunatley she did not appear to be when I was in her lair and then a group of Ghouls appeared. Luckily I was able to escape and make it back to town. I would like for you to take on this quest. I have this. (she pulls out a beautiful bejeweled silver comb) and I can give you three healing potions as payment. I will give you these before your quest so that they might aid you if needed."
        }
      ];
  $("document").ready(function(){
    $("#next").click(function(){
      let number = count
      let text = conversation[number].quote
      count = count + 1
      $("#said").html(text)
    });
    $("#conyberry").click(function(){
    });
  });
</script>
      
      
