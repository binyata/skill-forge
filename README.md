What I used to setup Nodejs v22.12.0

# installs fnm (Fast Node Manager)
winget install Schniz.fnm

# configure fnm environment (Using Powershell)
fnm env --use-on-cd --shell power-shell | Out-String | Invoke-Expression

# download and install Node.js
fnm use --install-if-missing 22

# verifies the right Node.js version is in the environment
node -v # should print `v22.12.0`

# verifies the right npm version is in the environment
npm -v # should print `10.9.0`