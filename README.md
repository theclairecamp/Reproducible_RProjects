# Reproducible_RProjects
Documenting protocol on how to create reproducible R projects

Utilizing procedure found on: https://appsilon.com/renv-how-to-manage-dependencies-in-r/

For more info on renv(): https://rstudio.github.io/renv/articles/renv.html

Procedure for creating reproducible environment:
1. Create R Project
2. Activate renv environment
3. Install all packages for that environment
4. Take snapshot to initalize documentation of environment
5. Run analyses and re-take snapshot to update documentation
6. Transfer to git repo

Procedure for restoring R environment from renv()
1. git clone https://github.com/theclairecamp/<project>.git NewRenvProject
2. Open project that was downloaded
3. Then run - renv::restore() - to restore the R environment that was created for initial project

*Note: When creating a snapshot, it will look through all the r files in your project, so if there are old files you will no longer use, place them in a different folder so those dependencies aren't created (i.e., have a parent folder that houses old code and your project folder)*
