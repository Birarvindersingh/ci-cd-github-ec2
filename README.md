<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
</head>
<body>

  <h1>💻 CI/CD Pipeline with GitHub Actions for EC2 Deployment</h1>

  <p>This project demonstrates how to automate the build and deployment processes on code changes to an Amazon EC2 instance using GitHub Actions.</p>

  <h2>🚀 Project Overview</h2>
  <ul>
    <li>Create a GitHub Actions workflow to automate the build and deployment process of a static web page (index.html)</li>
    <li>Use <code>scp</code> in GitHub Actions to securely transfer files to an EC2 instance</li>
    <li>Execute remote SSH commands to restart Apache Web Server services on the EC2 instance after deployment</li>
    <li>Secure the CI/CD pipeline using SSH keys for secure access</li>
  </ul>

  <h2>🛠️ Technologies Used</h2>
  <ul>
    <li>GitHub Actions - Automate the build, test, and deployment pipeline.</li>
    <li>Apache Web Server - Serve the static HTML web page.</li>
    <li>Amazon EC2 - Host the static website.</li>
    <li>SSH - Secure remote access to EC2 instance.</li>
    <li>YAML - Define CI/CD pipeline configuration.</li>
  </ul>

  <h2>⚙️ Workflow Overview</h2>
  <ul>
    <li><strong>Push to GitHub</strong>: Every time you push changes to the <code>main</code> branch, the workflow triggers automatically.</li>
    <li><strong>Build Process</strong>: The GitHub Actions workflow fetches the latest code (static <code>index.html</code> page).</li>
    <li><strong>File Transfer</strong>: Using <code>scp</code>, the <code>index.html</code> file is transferred to the EC2 instance.</li>
    <li><strong>Remote Execution</strong>: After file transfer, the workflow SSHs into the EC2 instance and restarts the Apache web server to serve the updated page.</li>
  </ul>

  <h2>📸 Project Screenshots</h2>
  <img src="https://github.com/Birarvindersingh/ci-cd-github-ec2/blob/main/1.PNG" alt="Screenshot 1" width="600" /> 
  <img src="https://github.com/Birarvindersingh/ci-cd-github-ec2/blob/main/2.PNG" alt="Screenshot 2" width="600" /> 
  <img src="https://github.com/Birarvindersingh/ci-cd-github-ec2/blob/main/3.PNG" alt="Screenshot 3" width="600" /> 
  <img src="https://github.com/Birarvindersingh/ci-cd-github-ec2/blob/main/4.PNG" alt="Screenshot 4" width="600" /> 
  <img src="https://github.com/Birarvindersingh/ci-cd-github-ec2/blob/main/5.PNG" alt="Screenshot 5" width="600" /> 
  <img src="https://github.com/Birarvindersingh/ci-cd-github-ec2/blob/main/6.PNG" alt="Screenshot 6" width="600" />

  <h2>🌐 Live Preview</h2>
  <p>Once deployed, you can visit the deployed site here:</p>
  <p>🔗 <a href="http://18.222.22.180">Instance URL</a></p>

</body>
</html>
