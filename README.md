# Kubernetes Hands-on sessie HHS

In deze handson-sessie zullen we kijken naar Kubernetes. Omdat het nogal een hassle is om alle dependencies te downloaden en te installeren zul je die downloaden tijdens het eerste gedeelte van de handson.

## Deel 0 (Download en installatie van dependencies, tijdens het wachten doe deel 1)
Download de volgende onderdelen specifiek voor jouw besturingssysteem en architechtuur. (Ik raad aan om deze handson te doen in een Linux-achtige omgeving omdat onder Windows dit vaak problemen oplevert.) 

1. Zorg dat je VT-x or AMD-v virtualisatie hebt geactiveerd in je BIOS.
2. Download en installeer [Virtualbox](https://www.virtualbox.org/wiki/Downloads)
3. Download en installeer [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
4. Download en installeer [minikube](https://github.com/kubernetes/minikube/releases)
5. Download en installeer Docker.

## Deel 1

Om je alvast wat indruk te geven hoe te werken met minikube heeft de Kubernetes website een online minikube tool gemaakt. Lees de onderstaande pagina's door en doe de intractieve tutorial die je kunt starten onderaan de pagina.

1. Zet het cluster op met minikube in [Module 1](https://kubernetes.io/docs/tutorials/kubernetes-basics/create-cluster/).
2. Deploy je eerste applicatie op minikube in [Module 2](https://kubernetes.io/docs/tutorials/kubernetes-basics/deploy-app/deploy-intro/).
3. Bekijk je deployment op het cluster in [Module 3](https://kubernetes.io/docs/tutorials/kubernetes-basics/explore/explore-intro/).
4. Expose je applicatie in [Module 4](https://kubernetes.io/docs/tutorials/kubernetes-basics/expose/expose-intro/).
5. Schaal je applicatie op in [Module 5](https://kubernetes.io/docs/tutorials/kubernetes-basics/scale/scale-intro/).
6. Doe een rolling-update van je applicatie in [Module 6](https://kubernetes.io/docs/tutorials/kubernetes-basics/update/update-intro/).

## Deel 2

Nu je een ervaren Kubernetes gebruiker bent kan het allemaal wat moeilijker worden. Ondertussen heb je de dependencies uit deel 0 ge"installeerd en ben je klaar om een cluster op te zetten. De eerste paar opgaven zullen nog wat tips geven maar het is de bedoeling dat je ook zelf op zoek gaat in de [documentatie](https://kubernetes.io/docs)

1. Zet een cluster op met minikube
2. Deploy een echoserver applicatie op je cluster. (Kijk naar het command `run` en de image die je nodig hebt staat hier: k8s.gcr.io/echoserver)
3. Expose de applicatie met een NodePort
4. Bekijk de applicatie in je browser
5. Verwijder de service
6. Verwijder de deployment
7. Sluit het cluster af

## Deel 3

Als je snel klaar bent met bovenstaande opgaven is er nog deze bonus opgave. Als ik eerlijk ben is dit eigenlijk de leukste opdracht maar ook de pittigste. Er is wat voorkennis nodig van Docker, maar dit kun je ook allemaal opzoeken in de Documentatie van Docker.

1. Maak een eigen Docker image (Ik raad aan om dit te doen op basis van een NGINX image om alleen wat statische html te serveren)
2. Maak een account op Docker hub en stuur daar je image heen
3. Deploy nu je eigen gemaakte image op het minikube cluster.


