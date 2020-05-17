PROIECT EGIOC 

RATIU ANDREI RAUL an 3 CTI , gr 5.2

Cu ajutorul bibliotecilor THREE JS am realizat :

-> o scena
-> o camera
-> 3 obiecte de tip Sphere pentru care am specificat dimensiunile si tipul de Mesh(material)
-> actiuni : click pe prima sfera , se schimba culoarea random (material3.color =new THREE.Color(0xffffff * Math.random());) si
	     se modifica wireframe( obiect plin sau doar frame-ul)
	     click pe a doua sfera , aceasta se deplaseaza vertical folosind 
				sphere.rotation.x = time * 4;
 				sphere.position.y = 0.5 + Math.abs(Math.sin(time * 2)) * 20	;
 				sphere.position.z = Math.cos(time) * 4; 
		trecand cu mouse-ul peste a 3-a sfera , aceasta se mareste 
->functia animate(): roteste sferele si permite zoom in sau zoom out , trateaza si evenimentul de bouncing pentru cea de a 2-ua sfera 