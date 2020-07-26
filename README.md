# README

Example stack: Constructs CodeBuild that is able to accessing build environment using Session Manager

For more details, you can see the article as follows.

- [AWS CodeBuild now supports accessing Build Environments with AWS Session Manager](https://aws.amazon.com/jp/about-aws/whats-new/2020/07/aws-codebuild-now-supports-accessing-build-environments-with-aws-session-manager/)
- [AWS CodeBuild - View a running build in Session Manager](https://docs.aws.amazon.com/codebuild/latest/userguide/session-manager.html)


## How I try it?

See [how-to-try-it.md](how-to-try-it.md).

## When should I use its feature? Is there effective use-cases?

I think that it should be use to debug or testing at develop phase.

For example, when you would like to fix version issue about language runtime or external packages.

Denotes some case uses.

- Does the runtime declaration by buildspec (at `install` phase) be applied to build environment correctly?
- Does the specific command works well in the build environemnt?
- Does the project environement works well as me expected?
- It looks like unexpected environment has applied in build phases (e.g. python virtualenv)