# Repro for Edge's iframe with sandbox="allow-scripts" bug

##Intall and run
```
npm install
npm run serve
```

browse http://localhost:8000/

##The problem
"Main" document adds some test cookie.
Iframe initialized with `sandbox="allow-scripts"` attribute.
Iframe makes XHR and main document's cookie is attached to request header.
