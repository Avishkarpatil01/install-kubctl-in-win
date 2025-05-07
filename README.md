#step 1
"https://dl.k8s.io/release/v1.33.0/bin/windows/amd64/kubectl.exe"

#step 2
curl.exe -LO "https://dl.k8s.io/v1.33.0/bin/windows/amd64/kubectl.exe.sha256"

#step 3
CertUtil -hashfile kubectl.exe SHA256
type kubectl.exe.sha256

#step 4
kubectl version --client
