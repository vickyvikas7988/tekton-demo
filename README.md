# tekton-demo
Tekton pipelines demo by building the image and pushing into the docker hub

<h2>Replace below params with appropriate values</h2>

<li>  git clone vickyvikas7988/tekton-demo</li>
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


