# over-engineered-todos
This is an example application created with purpose of learning and experimenting with new technologies. Thus it is meant to be over engineered solution to a simple ToDo list problem.

## Tech Stack
- Go for backend services
- Bazel

### Build instructions
```
    # This will update the dependencies of the specifid components go.mod file
    bazel run //:gazelle -- update-repos -from_file=[Path to go.mod file for that service]
    
    # this will update the Build.bazel file for all the components
    bazel run //:gazelle
    
    # This will build the specific component
    bazel build //services/[service folder]:[service name]
    
    # This will build all
    bazel build //...
    
    # This will run specific component
    bazel run //services/[service folder]:[service name]
```
