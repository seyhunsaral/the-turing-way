# Issue Tracking

Most projects have some kind of issue board to easily track certain aspects of the project, such as bug fixing, rolling out new features, or community engagement.
[GitHub](https://github.com) (a very popular collaboration platform) has a built-in [issue tracker](https://guides.github.com/features/issues/).
Issues can also be collated together into [project boards](https://help.github.com/en/github/managing-your-work-on-github/about-project-boards) to track progress towards a more specific, higher-level goal.

This section is a discussion around why you may keep issues and where you can store these issues.

## What is the purpose of your issues?

There are many different reasons for keeping/tracking issues related to a project and what your issues are tracking may influence how you present these to the wider community.

Are you using issues to track a central service?
Are they tracking personal to-do lists and being used to answer questions like if a task is high priority or if it is assigned to someone already.
This kind of tracking is best done in a centralised system and does not need to be circulated to your wider community.

If you're using issues to track bug reports, feature requests, opportunities for community members to engage, and so on, then a public issue board will allow your community to get a clear overview of what's coming down the pipeline and how they can get involved.

If your project is split across multiple repositories, then it's a good idea to keep the issues specifically relating to that module within that repository.
This allows your community to focus their attention on what is important to them.

Let's look into centralised and decentralised/distributed issue boards and how they might engage your community.

### Issues per Repository (Decentralised/Distributed)

This approach has several smaller issue boards for each repository (or module) within your codebase.
This method has a lot of positive outcomes, such as:

- The volume of issues is more manageable;
- Most contributors only need to be aware of issues relating to one or two repositories;
- Contributors can subscribe to notifications or updates from only the repositories that interest them;
- It feels like "divide and conquer", more people are working on more aspects to move the project as a whole forward.

#### Case study: mybinder.org

[mybinder.org](https://mybinder.org) is a platform facilitating users to easily share reproducible analyses and computational environments with one another in [Jupyter Notebooks](https://jupyter-notebook.readthedocs.io/en/stable/) via the cloud.
This project is spread across a number of different repositories, each one an individual tool that can be used in isolation from the others.
These are:

- [repo2docker](https://github.com/jupyter/repo2docker),
- [JupyterHub for Kubernetes](https://github.com/jupyterhub/zero-to-jupyterhub-k8s),
- [BinderHub](https://github.com/jupyterhub/binderhub).

Each of these repositories contains hundreds of issues tracking on-going work being performed by the community and scoping future directions for each project to take.

Can you imagine trying to combine all of these issues into one place?
It would become very difficult, if not impossible, for someone to find what they are looking for and would require a very clever tagging schema plus instructions for filtering by tag.

In the Project Binder team's experience, most community members contribute to just one or maybe two of these projects.
So having consolidated access to all the issues for all the working parts is not a high priority for their community.

They find that having distributed issue tracking allows those members of the community who may only work with JupyterHub to comfortably contribute without needing to be familiar with everything that goes into running [mybinder.org](https://mybinder.org).

### Centralised Issue Repository

With a big project, it can be tempting to collate all your issues into one place for the sake of easier management.
However in terms of engaging your community, this can be problematic.
If your issues are elsewhere this can create a lot of barriers to entry for community members, such as:

- Issues are more difficult to discover;
- If they are hosted on another platform, that's another thing community members need to learn how to use;
- Issues are separate to the code they are referencing.

A very large impact on the community of having a separate issue repository is that when people visit your code repository, it looks like an inactive project because there are no issues or conversations going on where the code is hosted.
This may cause community members to believe that the code is no longer being actively developed/maintained/supported and may choose to use another codebase or software package.

## Comparative Table

| Feature | Single Issue Repo | Issue Tracker per Repo |
| :--- | :---: | :---: |
| Global issue search | ✅ | |
| Hosted by the same Platform | ❓(not guaranteed) | ✅ |
| Filter by repository | ❓(power users*) | ✅ |
| Suscribe to relevant updates | ❓(power users) | ✅ |
| Easy to Discover | | ✅ |
| Connected to the Codebase | | ✅ |
| Appears active to community | | ✅ |
| Manageable volume | | ✅ |

*Power users = These are people who are already familiar enough with a platform to know the gotchas and tricks that make their experience more efficient