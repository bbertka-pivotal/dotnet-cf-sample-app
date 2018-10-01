# pcf-dotnet-environment-viewer

Push the app using manifest defaults, cd into the environment folder that holds the app code:
```
cd ViewEnvironment
```

Update the manifest.yml file to have a route that cooresponds to your email handle, for example:

Note: you should use Notepad++ or code text editor for edits to YML
```
applications:
- name: dotnet-example
  host: dotnet-bbertka
  memory: 128M
  stack: windows2012R2
  instances: 1
  buildpack: hwc_buildpack
```

Push your application:
```
cf push
```
