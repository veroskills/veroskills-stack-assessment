# VeroSkills Engineer Assessment

VeroSkills uses the [T3 Stack](https://create.t3.gg/), and this repository is a new app scaffolded with `create-t3-app`. The stack is made up of:

- [Next.js](https://nextjs.org)
- [NextAuth.js](https://next-auth.js.org)
- [Prisma](https://prisma.io)
- [Tailwind CSS](https://tailwindcss.com)
- [tRPC](https://trpc.io)

Prior to your assessment, feel free to familiarize yourself with the docs for these technologies. When the assessment begins we will give you the `DATABASE_URL` for your `.env`, and a `GITHUB_CLIENT_ID` and `GITHUB_SECRET` for NextAuth's GitHub provider.

**Please make sure that you prioritize typesafety.** Unless absolutely necessary we do not want to see any `any` types in your code. Instead we want to see how you will help to create a safe and reliable codebase, even if it takes more time to do it correctly.

## Assessement

We could throw a set of LeetCode or CoderByte assessments at you, but our philosophy is that engineers should think less about abstract coding challenges and more about how to solve real world problems for users. With that in mind, we want to see your ability to grasp the basics of our stack, and how you would approach creating a simple link shortener.

## Requirements

- Users must be signed-in in order to create a link. How will you handle this?
- On the `index` page, display a form that allows users to enter a URL and a custom slug. The slug should be optional, and if it is not provided, a random slug should be generated. Will you use a library for form management, or is there a more effective solution?
- Using tRPC, create a mutation that will create a new record in the database. Make sure to validate the URL and slug, and return any errors to the user. Ensure that the slug is unique, and the URL is related to the current user.
- Using tRPC, create a query that will render all of a user's links on the client.
- Create a page that will redirect to the original URL when a user visits the custom slug.

### Notes

You can install any new packages that you feel are necessary to complete the assessment, and please, by all means, use Google, Stack Overflow, and GitHub Copilot to your advantage; every engineer today does it, and we want to see how you think about problems, not how much syntax you have memorized. You'll have about 30 minutes to get as much done as possible, and we are looking at how you approach the problem, and how you think about the stack.