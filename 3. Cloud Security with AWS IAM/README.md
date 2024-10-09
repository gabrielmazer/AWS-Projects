# AWS IAM and Cloud Security Project

In this project, I focused on using **AWS Identity and Access Management (IAM)** to secure AWS resources. My goal was to manage access to **EC2 instances** by configuring IAM policies, users, and user groups, ensuring proper permissions based on the environment (production vs development).

## Documentation:
You can view the full project documentation, including all visualizations and analysis, in this [PDF](https://gabrielmazer.github.io/AWS-Projects/IAM.pdf).

## What I Did

- **Created IAM Policies**: I built custom JSON-based policies to control which actions can be performed on EC2 instances, depending on their tags (production or development).
- **Managed IAM Users and Groups**: I configured IAM user groups to simplify permissions management for multiple users and attached policies to ensure consistent access control.
- **Tagged EC2 Instances**: I assigned `Env` tags to EC2 instances to classify them as production or development, allowing for environment-specific permissions.
- **Tested Access Control**: I tested the policies by logging in as a new IAM user and attempting actions on the EC2 instances to verify the permissions.
- **Used Policy Simulator**: I also used the IAM Policy Simulator to validate the effectiveness of my policies without directly affecting the resources.

## Tools and Services Used

- **AWS IAM**: For managing users, user groups, and creating access policies.
- **Amazon EC2**: For launching and managing cloud instances.
- **IAM Policy Simulator**: To test and validate my policies.

## Key Insights

- **Custom IAM Policies**: I created policies that allowed actions like starting or stopping EC2 instances in development environments while restricting actions in production.
- **User Group Management**: By using IAM user groups, I streamlined permissions management across multiple users, ensuring that the right people have access to the right resources.
- **Tags for Better Organization**: By tagging EC2 instances as production or development, I ensured that permissions were tied to the environment, enhancing security and organization.
- **Hands-On Policy Testing**: I tested permissions by performing actions like stopping instances, where production restrictions applied, and development actions succeeded.

## Project Breakdown

1. **Set Up EC2 Instances**: I created two EC2 instances, tagging one as `production` and the other as `development` for environment-specific access control.
2. **Defined IAM Policies**: I wrote a custom JSON policy that allowed full access to EC2 instances tagged `development` but restricted actions on `production` instances.
3. **Configured IAM User Groups**: I created a user group, attached the policy, and added new IAM users, ensuring they inherited the appropriate permissions.
4. **Tested Permissions**: I logged in as a new IAM user and tested actions such as stopping the EC2 instances. The policy worked as expected: production actions were denied, and development actions succeeded.
5. **Validated with the Policy Simulator**: I used the IAM Policy Simulator to ensure my policy was correctly written and applied, allowing me to verify access without affecting live resources.

## Conclusion

This project gave me hands-on experience with AWS IAM, allowing me to refine my skills in creating and applying access policies, managing user groups, and securing cloud resources. By using EC2 tags and role-based access controls, I ensured that only authorized actions could be performed, based on the environment. It was a great learning opportunity to explore AWS security best practices, and I look forward to applying these skills in larger cloud environments.

