
<!DOCTYPE HTML>
<html lang="en">
    <head>
		<title>Meo.my Scope</title>
		<meta charset="utf-8">
		<meta name="viewport" content="width=device-width; initial-scale=1.0; maximum-scale=1.0; user-scalable=0;"/>
		<style type="text/css">
			body {
				background-color: #000000;
				margin: 0px;
				overflow: hidden;
			}

			a {
				color:#0078ff;
			}
		</style>
	</head>
	<body>

		<script type="text/javascript" src="js/Three.js"></script>
		<script type="text/javascript" src="js/Particle3D.js"></script>
		<script type="text/javascript" src="js/Stats.js"></script>

		<script type="text/javascript">
        
        // based on a demo at http://sebleedelisle.com/demos/GravityParticles/ParticlesForces3D.html

			var container, stats;
			var camera, scene, renderer, particle;
			var mouseX = 0, mouseY = 0;
			var particles = [],
				MAX_PARTICLES = 100;
			 

			var windowHalfX = window.innerWidth / 1.5;
			var windowHalfY = window.innerHeight / 1.5;

		

			function addPart(){
				makeParticle(1); 
				if(particles.length<MAX_PARTICLES)
					setTimeout(addPart, 50); 

			}


			init();
			setInterval( loop, 1000 / 60 );

			function init() {

				container = document.createElement('div');
				document.body.appendChild(container);

				camera = new THREE.Camera( 75, window.innerWidth / window.innerHeight, 1, 3000 );
				camera.position.z = 100;

				scene = new THREE.Scene();

				

				renderer = new THREE.CanvasRenderer();
				renderer.setSize( window.innerWidth, window.innerHeight );
				container.appendChild( renderer.domElement );

				stats = new Stats();
				stats.domElement.style.position = 'absolute';
				stats.domElement.style.top = '0px';
				container.appendChild( stats.domElement );

				document.addEventListener( 'mousemove', onDocumentMouseMove, false );
				document.addEventListener( 'mousedown', onDocumentMouseDown, false );
				document.addEventListener( 'touchstart', onDocumentTouchStart, false );
				document.addEventListener( 'touchmove', onDocumentTouchMove, false );
		
				addPart();
			}

			//

			function onDocumentMouseMove( event ) {

				mouseX = event.clientX - windowHalfX;
				mouseY = event.clientY - windowHalfY;
			}
			function onDocumentMouseDown( event ) {

				makeParticle(); 
			}
			function onDocumentTouchStart( event ) {

				if ( event.touches.length == 1 ) {

					event.preventDefault();

					mouseX = event.touches[ 0 ].pageX - windowHalfX;
					mouseY = event.touches[ 0 ].pageY - windowHalfY;
				}
			}

			function onDocumentTouchMove( event ) {

				if ( event.touches.length == 1 ) {

					event.preventDefault();

					mouseX = event.touches[ 0 ].pageX - windowHalfX;
					mouseY = event.touches[ 0 ].pageY - windowHalfY;
				}
			}

			//

			function loop() {


				var repelforce = new THREE.Vector3(0,0,0),
					mag, 
					repelstrength; 

				for (i=0; i<particles.length; i++){
					var p1 = particles[i]; 

					repelforce.copy(p1.position);
	 				
					mag = repelforce.length(); 
	 				repelstrength = (mag - 100) *-0.1; 

	 				if(repelstrength<0)  {
						repelforce.multiplyScalar(repelstrength/mag);
						p1.force.addSelf(repelforce); 
					}
					
					if(i>=particles.length-1) continue; 
					
					for(j=i+1; j<particles.length; j++) {
						var p2 = particles[j];

						repelforce.copy(p2.position); 
						repelforce.subSelf(p1.position); 
						mag = repelforce.length(); 
						repelstrength = 50-mag; 

						if((repelstrength>0)&&(mag>0))	{

							repelforce.multiplyScalar(repelstrength*0.05 / mag); 

							p1.force.subSelf(repelforce); 
							p2.force.addSelf(repelforce); 

						}
					}


				}


			  	// iteratate through each particle
				for (i=0; i<particles.length; i++){
					var particle = particles[i]; 

					particle.update();

				
				}



				camera.position.x += ( mouseX - camera.position.x ) * 0.05;
				camera.position.y += ( - mouseY - camera.position.y ) * 0.05;

				renderer.render( scene, camera );

				stats.update();
			}
			
			
			function makeParticle(){
				
				var color = Math.random() * 0x808008 + 0x808080; 
				particle = new Particle3D( new THREE.ParticleCircleMaterial( { color: color, opacity: 1 } ) );
		
				particle.scale.x = particle.scale.y = 5;
				scene.addObject( particle );
			
				particle.position.set(0,0,0); 
				particle.velocity.set(1,0,0);
				particle.velocity.rotateZ(Math.random()*90);
				particle.velocity.rotateY(Math.random()*360); 
			
				particle.drag = 0.96;
		
			
				particles.push(particle); 
				
				
			}
			

		</script>
	</body>
</html>

