perfecthalf = ((1 / 37) * 360) / 2;

let currentLength = perfecthalf;

$(".wheel img").css("transform", "rotate(" + perfecthalf + "deg)");

$(".spin").click(() => {
  $(".wheel img").css("filter", "blur(8px)");

  spininterval = getRandomInt(0, 37) * (360 / 37) + getRandomInt(3, 4) * 360;
  currentLength += spininterval;

  numofsecs = spininterval;

  console.log(currentLength);
  $(".wheel img").css("transform", "rotate(" + currentLength + "deg)");

  setTimeout(function () {
    $(".wheel img").css("filter", "blur(0px)");
  }, numofsecs);
});

function getRandomInt(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

$(document).ready(function() {
  $(".spin").click();
})