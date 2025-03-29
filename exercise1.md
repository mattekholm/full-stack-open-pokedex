# Exercise 1

## Tools for linting, testing, and building in C#

In my (limited) experience, .NET provides decent tooling out of the box, such as the Roslyn compiler, which handles linting. However, there are also other popular options, such as JetBrains ReSharper, SonarQube, and StyleCop Analyzers.

## Alternative CI tools besides Jenkins and GitHub Actions

There are a number of alternatives, including Azure Pipelines, Bitbucket Pipelines, Bamboo, AWS CodePipeline, GitLab, CircleCI, TeamCity, and more.

## Would this setup be in a self-hosted or a cloud-based environment? Why? What information would be needed to make the decission?

Deciding between a self-hosted or cloud-based environment depends on the type of project. As mentioned in the lectures, for smaller projects, it is most likely easier (and probably cheaper) to choose a cloud-based environment. For larger projects, where privacy may be a concern, or when specific dependencies or hardware are required, or where build times are expected to be very long, it might be better to use on-premises hardware.

Out of convenience, I would easily choose the cloud-hosted option if possible, to avoid having to maintain the server and instead focus on defining the workflow. However, I have also encountered a situation where cloud hosting was not a possibility. I was building a component that depended on a licensed COM API. In this case, an on-premises agent would have made more sense (had I chosen to implement a CI/CD pipeline).

--

*MH, 2025*
