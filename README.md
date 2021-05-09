# tekton-demo - kubernetes - OCI (Oracle Cloud Infrastructure)
Tekton pipelines demo - Building the image using Dockerfile present in GitHub and pushing into the Docker Hub

 <h3> <b>Code is placed in GitHub ---> Kaniko Image is pulled into OCI --->  Kaniko is used to Build Container Images In Kubernetes ---> Finally, pushing image to Docker Hub  </b> </h3>
 
<b>Note - Replace below params with appropriate values</b>

$ git clone vickyvikas7988/tekton-demo
<br>

<ul>
<li> In git-resource.yaml replace github-username/github-repository with your git username and git repository </li>
<li> In docker-resource.yaml replace docker-username/docker-repository with your docker username and docker repository</li>
<li> In docker-secret.yaml file modify repalce-with-your-username, replace-with-your-password </li>
</ul>

<p> Once you modify above values, please follow below steps </p>
<ol>
<li> cd tekton_files/ </li>
<li> kubectl apply -f ./*</li>
<li> tkn taskrun logs build-docker-image-from-git-task-run</li>
</ol>


