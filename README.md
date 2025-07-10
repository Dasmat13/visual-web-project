<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Kubernetes Animated Website - Project Info</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: #f8f9fa;
      margin: 0;
      padding: 2rem;
      line-height: 1.6;
      color: #333;
    }
    h1, h2, h3 {
      color: #005f73;
    }
    code {
      background: #eee;
      padding: 0.2em 0.4em;
      border-radius: 4px;
    }
    pre {
      background: #eee;
      padding: 1em;
      overflow-x: auto;
      border-radius: 6px;
    }
    .section {
      margin-bottom: 2rem;
    }
    .folder-structure {
      font-family: monospace;
      background: #f1f1f1;
      padding: 1rem;
      border-radius: 5px;
    }
    .highlight {
      background-color: #e0f7fa;
      border-left: 4px solid #00bcd4;
      padding: 1em;
      margin: 1em 0;
    }
    a {
      color: #0077b6;
    }
  </style>
</head>
<body>

  <h1>🚀 Visual Web Project – Kubernetes Animated Website</h1>

  <div class="section">
    <p>This project demonstrates a visually appealing <strong>animated website</strong> deployed using <strong>Docker</strong> and <strong>Kubernetes (Minikube)</strong>.</p>
    <p>It features a simple static site with animated CSS and JavaScript, containerized using <strong>Nginx</strong>, and deployed via a <strong>Kubernetes Deployment, Namespace, and Service</strong>.</p>
  </div>

  <div class="section">
    <h2>🌐 Live Demo (Minikube)</h2>
    <div class="highlight">
      You can access the site locally via:<br />
      <code>http://localhost:&lt;NodePort&gt;</code> after deploying using Minikube
    </div>
  </div>

  <div class="section">
    <h2>🧱 Tech Stack</h2>
    <ul>
      <li>🧾 HTML, CSS (Animated)</li>
      <li>🔌 JavaScript</li>
      <li>🐳 Docker (Nginx)</li>
      <li>☸️ Kubernetes (Minikube)</li>
      <li>💻 YAML for deployment</li>
    </ul>
  </div>

  <div class="section">
    <h2>📁 Folder Structure</h2>
    <pre class="folder-structure">
visual-web-project/
├── index.html           # Main animated page
├── style.css            # CSS gradient animation
├── script.js            # JS console log
├── Dockerfile           # Containerizes site with Nginx
├── namespace.yaml       # Creates hello-kubernetes namespace
├── deployment.yaml      # Deploys container in Kubernetes
└── service.yaml         # Exposes app via NodePort on port 8080
    </pre>
  </div>

  <div class="section">
    <h2>🚀 How to Run It</h2>
    <h3>1️⃣ Clone the Repo</h3>
    <pre><code>git clone https://github.com/Dasmat13/visual-web-project.git
cd visual-web-project</code></pre>

    <h3>2️⃣ Build and Push Docker Image</h3>
    <pre><code>docker build -t dasmat13/kube-animated-site .
docker push dasmat13/kube-animated-site</code></pre>

    <h3>3️⃣ Start Minikube and Apply Manifests</h3>
    <pre><code>minikube start

kubectl apply -f namespace.yaml
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml</code></pre>

    <h3>4️⃣ Access the Website</h3>
    <pre><code>minikube service hello-service -n hello-kubernetes</code></pre>
    <p>Or manually:</p>
    <pre><code>kubectl get svc -n hello-kubernetes</code></pre>
    <p>Then open: <code>http://localhost:&lt;NodePort&gt;</code></p>
  </div>

  <div class="section">
    <h2>📸 Screenshot or Preview</h2>
    <p><em>No screenshot added by choice. Website features animated CSS gradients and centered content.</em></p>
  </div>

  <div class="section">
    <h2>📜 License</h2>
    <p>MIT License</p>
  </div>

  <div class="section">
    <h2>🙋‍♂️ Author</h2>
    <p><a href="https://github.com/Dasmat13" target="_blank">@Dasmat13</a></p>
  </div>

</body>
</html>
