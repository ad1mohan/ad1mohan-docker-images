## Usage of setting color
* As a command line argument with --color as the argument. Accepts one of red,green,blue,blue2,pink,darkblue 
* As an Environment variable APP_COLOR. Accepts one of red,green,blue,blue2,pink,darkblue

### Available colors
```
red
green
blue
blue2
pink
darkblue
```

### Docker run
```
docker run --name web-color-container -p 80:8080 -d ad1mohan/web-color-app 
```

### Kubernetes pod yaml
```
...
spec:
  containers:
  - env:
    - name: APP_COLOR
      value: pink
...
```