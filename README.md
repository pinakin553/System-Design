# System-Design

### Can you design a scalable system like YouTube or Zomato where traffic doesn't crash your servers?
Expected Talking Points:
- Step 0: Most effective and optimized Load balancing is a key component here
- Step 1: When a client sends a request (req1, req2,...), the LB catches it before it hits the backend
- Step 2: It looks at the current load across servers and decides which one to forward a request to.
- Step 3: Make sure to mention the type of Load balancing algorithm and the type of Load balancer (hardware or software) that will be used
- Step 4: Make sure to mention - "I would also integrate health checks with my Load balancer to ensure traffic only hits active, responsive servers.
- Step 5: Load Balancer is our system's first line of defense during high traffic days

### Can you design and automate Terraform commands in a pipeline (CI/CD)?
Expected Discussion Points:
- Step 0: Use a wrapper script or tools like Terragrunt, Atlantis, or Spacelift
- Step 1: Locking via S3 + DynamoDB
- Step 2: Use terraform plan-out + approval step
- Step 3: Linting/formatting/validation checks
- Step 4: Secrets handling via Vault or SSM

### How would you ensure safe and auditable Terraform usage across teams?
Expected Talking Points:
- Step 0: Enforce peer-reviewed PRs with terraform plan output
- Step 1: Use remote backends with locking
- Step 2: Use workspaces or separate states per environment
- Step 3: Role-based access via IAM
- Step 4: Use pre-commit hooks or pipelines to check fmt, validate
