# sfdx-module-template
Place folder structure inside of force-app/main/.

# branches
## master
Used to deploy into the production environment.

## stg
Used to deploy into the **staging environment**. A Salesforce staging environment (**STG**) should be a full copy sandbox org. It's purpose is to test code, builds and updates to ensure quality in an environment that closely resembles the production environment. User acceptence testing (UAT) is to be done in this environment to limit unwanted deployments to production. Once UAT & QA is complete and accepted, promote all changes to the **production environment**.

## int
Used to deploy into the **integration environment**. A Salesforce integration environment (**INT**) should be a partial copy sandbox org. It's purpose is to combine and validate the work of the entire project so that QA can run their tests before the work is promoted to the **staging environment**.

## dev
Used to deploy into the **development environment**. A Salesforce development environment (**DEV**) should be a developer org. It's purpose is to develop source code, packages or make administration changes to SFDC. This should be a combination of feature branches and validated by QA before the work is promoted to the **integration environment**.
