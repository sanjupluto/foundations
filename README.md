# foundations
multi‑module Maven project


✅ Key Rule
- Only the root parent project should extend spring-boot-starter-parent.
- Child modules should extend your parent project.
- This way, all child modules inherit Spring Boot’s dependency management and plugin configuration through the parent, keeping things consistent.

🔑 Why This Matters
- Keeps version management centralized (Spring Boot version defined once in parent).
- Prevents conflicts if different modules try to use different Spring Boot parents.
- Makes builds cleaner and easier to maintain.
