# Dump all links

Array.from(document.querySelectorAll("a")).forEach(function(itm){
  console.log(itm.getAttribute('href'));
});


