# snyk-workflows

use Reusable Workflow from Github see link below.

reusable workflow (file `snyk_pipenvv_monitor.yml`) that lives in it's own repo and gets called by the file that goes in the repo being scanned (file `snyk_pipenv_monitor2.yml`)

This essentially modularizes it as well as centralizes the workflow. The benefit of this is if you need to make changes to the workflow, it only exists in one place and you don't have to update it across many repos

In file `snyk_pipenv_monitor2.yml` you must replace `org-id-goes-here` with your Snyk org ID and `path-to-workflow-goes-here` with the path to the workflow in the other repo
