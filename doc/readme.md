A console client for reading data off TFS

## Educational goals

* Learn to interact with a web API from Python
* Learn more advanced `argparse` features

## MVP features

### Listing
The `list` option lists projects and tasks.  
Example: 
* `list --project <project name>` displays the task list for the project.
* `list` displays all the projects available. 

### Statistics
The `stat` option reads task/project/total history between selected dates
* the date is today if nothing else provided
* otherwise the date's controlled by the options `--start`, `--end`
* default verbosity level is `--total`
* to specify deeper nested levels please use `--project` or `--task`,
    these should be followed by the project name or task number

### Configuration
The `config` option caches data from the repo - how to deal with auth?  

### Miscellaneous  
* *Write logs* to stderr if a `-debug` option is given
