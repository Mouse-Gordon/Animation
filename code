<!doctype html>
<html lang="en">
<head>
 <title>Particle System</title>
 <meta charset="utf-8">
 <style>
canvas {
 border: 1px solid black;;
}
</style>
 <script>
 
 
 var canvas;
 var context;
 var particles;
 var particlesTwo;
 var timer;
 var Square;
 
 

 function makeBackground(){
     context.fillStyle = "black";
	 context.fillRect(0, 0, canvas.width, canvas.height);
	 context.globalCompositeOperation = "soure-over";
	
	  context.beginPath();
      context.moveTo(110, 20);
      context.bezierCurveTo(50, 20, 60, 70, 150, 70);
      context.bezierCurveTo(170, 100, 240, 100, 260, 70);
      context.bezierCurveTo(340, 60, 350, 50, 300, 20);
      context.bezierCurveTo(350, -40, 260, -50, 360, -30);
      context.bezierCurveTo(230, -75, 265, -60, 260, -30);
      context.bezierCurveTo(120, -75, 70, -60, 100, 20);

      // complete custom shape
      context.closePath();
      context.lineWidth = 5;
	  context.fillStyle = "grey";
	  context.fill();
      context.strokeStyle = 'grey';
      context.stroke();
 
 
 }
 
 
 function makeParticles() {
	//create an array of particles for our animation
	particles = [];
	for(var i = 0; i < 30; i++)
	{
		particles.push(new Particle());
	}
 }
  
 
 function degreesToRadians(degrees) {
	 //converts from degrees to radians and returns
	 return (degrees * Math.PI)/180;
 }
 function Particle()
 {
	 //the constructor for a single particle, with random starting x+y, velocity, color, and radius
	 this.x = 100;
	 this.y = canvas.height;
	 this.vx = Math.random()*10-5;
	 this.vy = Math.random()*10-5;
	 var colors = ["red", "orange"];
	 this.color = colors[Math.floor(Math.random()*colors.length)];
	 this.radius = 20;
 }
 



 function moveParticles() {
	 //partially clear the screen to fade previous circles, and draw a new particle at each new coordinate
	
	
	 
	 
	 //context.fillStyle = "black";
	 //context.fillRect(0,0,canvas.width,canvas.height)
	 //context.globalCompositeOperation = "destination-over";
	 //context.fillStyle = "rgba(0, 0, 0, .05)";
	 //context.fillRect(0, 0, canvas.width, canvas.height);
	 //context.globalCompositeOperation = "lighter";
	 for(var i = 0; i < particles.length; i++)
	 {
		 var p = particles[i];
		 context.beginPath();
		 context.arc(p.x, p.y, p.radius, 0, degreesToRadians(360), true);
		 context.fillStyle = p.color;
		 context.fill();
		 p.x += p.vx;
		 p.y += p.vy;
		 //if(p.x < -50) p.x = canvas.width+10;
		 //if(p.y < -50) p.y = canvas.height+10;
		 //if(p.x > canvas.width+10) p.x = -50;
		 //if(p.y > canvas.height+10) p.y = -50;
	 }
	
 }
 
 
 
  
function makeParticlesTwo() {
	//create an array of particles for our animation
	particlesTwo = [];
	for(var i = 0; i < 30; i++)
	{
		particlesTwo.push(new ParticleTwo());
	}
 }
  
 
 function degreesToRadians(degrees) {
	 //converts from degrees to radians and returns
	 return (degrees * Math.PI)/180;
 }
 function ParticleTwo()
 {
	 //the constructor for a single particle, with random starting x+y, velocity, color, and radius
	 this.x = 400;
	 this.y = canvas.height;
	 this.vx = Math.random()*10-5;
	 this.vy = Math.random()*10-5;
	 var colors = ["red", "orange",];
	 this.color = colors[Math.floor(Math.random()*colors.length)];
	 this.radius = 10;
 }
 



 function moveParticlesTwo() {
	 //partially clear the screen to fade previous circles, and draw a new particle at each new coordinate
	
	
	 
	 
	 //context.fillStyle = "black";
	 //context.fillRect(0,0,canvas.width,canvas.height)
	 //context.globalCompositeOperation = "destination-over";
	 //context.fillStyle = "rgba(0, 0, 0, .2)";
	 //context.fillRect(0, 0, canvas.width, canvas.height);
	 //context.globalCompositeOperation = "lighter";
	 for(var i = 0; i < particlesTwo.length; i++)
	 {
		 var p = particlesTwo[i];
		 context.beginPath();
		 context.fillRect(p.x, p.y, 40, 40, true);
		 context.fillStyle = p.color;
		 context.fill();
		 p.x += p.vx;
		 p.y += p.vy;
		 //if(p.x < -50) p.x = canvas.width+10;
		 //if(p.y < -50) p.y = canvas.height+10;
		 //if(p.x > canvas.width+10) p.x = -50;
		 //if(p.y > canvas.height+10) p.y = -50;
	 }
	
 }
   
 
 
    var can, ctx, step = 10, steps = 50;
              delay = 20;
   
 function init() {
          
            context.fillStyle = "blue";
            context.font = "10pt Helvetica";
            context.textAlign = "center";
            context.textBaseline = "middle";
            TextSmallToBig();
        }
        function TextSmallToBig() {
            step++;
            context.clearRect(0, 0, canvas.width, canvas.height);
            context.save();
            context.translate(canvas.width / 2, canvas.height / 2);
            context.font = step + "pt Helvetica";
            context.fillText("Fire", 0, 0);
            context.restore();
            if (step < steps)
                var t = setTimeout('TextSmallToBig()', 20);
        }  
		function customShap(){
		
			
		
		
		
		
		}
		
  function lightning(){
      context.beginPath();
      context.moveTo(135, 35);
      context.lineTo(135,35);
	  context.lineTo(100,40);
	  context.lineTo(50,80);
	  context.lineTo(90,220);
	  context.lineTo(100,400);
	  context.lineTo(110,220);
	  context.lineTo(70,80);
	  context.lineTo(135,35);
	  
	  context.fillStyle="yellow";
	  context.fill();
      context.stroke();
	  //context.globalCompositeOperation = "lighter";
	  }
	  
	   function lightningTwo(){
      context.beginPath();
      context.moveTo(250, 35);
      context.lineTo(250,155);
	  context.lineTo(300,200);
	  context.lineTo(330,280);
	  context.lineTo(420,430);
	  context.lineTo(360,300);
	  context.lineTo(350,240);
	  context.lineTo(260,150);
	  context.lineTo(250,35);
	  
	  context.fillStyle="yellow";
	  context.fill();
      context.stroke();
	  //context.globalCompositeOperation = "lighter";
	  }
		
   
 window.onload = function() {
 	 var timer2;
	 var timer3;
	 var timer4;
	 var timer5;
	 var timer6;
	 var timer7;
	 canvas = document.getElementById('canvas');
	 context = canvas.getContext('2d');
	 //makeText();
	 //makeParticlesTwo();
	 //makeParticles();
	 //makeParticles();
	 //makeParticlesTwo();
	init();
	lightning();
	 timer6 = setInterval(makeBackground,2800);
	 timer = setInterval(moveParticles, 50);
	 timer2 = setInterval(moveParticlesTwo, 50);
	 timer3 = setInterval(makeParticles,2850);
	 timer4 = setInterval(makeParticlesTwo,4000);
	 timer5 = setInterval(lightning,2850);
	 timer5 = setInterval(lightningTwo,4000);
	 
	 
	 }

</script>
</head>
<body>
	<canvas id="canvas" width="500" height="400"></canvas>
</body>
</html>
