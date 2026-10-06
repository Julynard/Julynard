<div align="center">

<img src="./assets/profile-header.svg" alt="Julynard Tago-on, Laravel / PHP Full-Stack Engineer" width="100%">

<p>
  <a href="https://julynardtago-on.netlify.app/"><img src="https://img.shields.io/badge/Website-315A9B?style=flat-square&logo=googlechrome&logoColor=white" alt="Julynard Tago-on's portfolio website"></a>
  <a href="https://www.linkedin.com/in/julynard-tago-on/"><img src="https://img.shields.io/badge/LinkedIn-0A8ACB?style=flat-square&logo=linkedin&logoColor=white" alt="Julynard Tago-on on LinkedIn"></a>
  <a href="https://www.facebook.com/julynard10/"><img src="https://img.shields.io/badge/Facebook-1877F2?style=flat-square&logo=facebook&logoColor=white" alt="Julynard Tago-on on Facebook"></a>
</p>

</div>

# Julynard Tago-on

**Laravel / PHP Full-Stack Engineer** in Dasmariñas, Cavite, Philippines, working remotely.

I'm a Laravel / PHP full-stack engineer focused on building reliable business applications, APIs, and workflow-driven systems.

## About

I've worked with Laravel and PHP for six years. Since February 2024 I've been a full-stack developer at CoreProc Inc., where I've shipped features across 12 client applications in retail loyalty, field sales, payments, e-commerce and SaaS. Before that I automated an expense-approval workflow for a government research agency (DOST-PCIEERD), built survey and quiz systems for the Philippine Statistics Authority, customised NetSuite for finance teams at CloudTech ERP, and built a ticket management system for Dinoland.

The problems I'm most useful on sit between the business process and the database: taking an approval chain, a reconciliation process or a subscription model and turning it into an application with clear rules, then keeping it fast and dependable once real data and real users arrive. I lead features from the design spec to production, review pull requests, and fix production incidents when they happen.

## Engineering focus

- **Laravel and PHP application design.** Controllers that only deal with HTTP, business rules in services, validation in Form Requests, response shape in API Resources. Laravel 5.8 through 12, Nova, Horizon and queues.
- **REST APIs and integrations.** Token-authenticated APIs with Sanctum, and integrations with Salesforce, PayPal subscriptions, PayMaya, Google OAuth/SSO and SFTP data feeds.
- **Workflow-driven business systems.** Approval flows, payment reconciliation, ticket and purchase-order lifecycles, audit trails and scheduled jobs.
- **Database design and performance.** MySQL schemas and views, multi-tenant data, indexing, removing N+1 queries, and moving slow exports onto queued, chunked jobs.
- **Frontends.** Vue 2 and 3 with Inertia.js, Livewire, Tailwind CSS.
- **Authentication and authorization.** Session auth for admin areas, API tokens, Google SSO, and roles and permissions enforced through policies.
- **Testing and quality.** PHPUnit and Pest feature tests, PHPStan with Larastan, PHP_CodeSniffer and Laravel Pint in CI.
- **Production support.** Tracing incidents such as a login redirect broken by a library upgrade, a failed data sync for multi-district supervisors, and payment-gateway failures back to their cause.

<img src="./assets/skills-v6.svg" alt="Skills: PHP, Laravel, Nova, Horizon, REST APIs, Vue.js, Inertia.js, MySQL, Redis, Salesforce, PayPal, PayMaya, AWS S3, Docker, Jenkins, PHPUnit, PHPStan and Laravel Pint" width="100%">

## Selected public work

Most of my professional work is client code I can't publish. These public repositories are where you can read my code directly.

### [Laravel User Management API](https://github.com/Julynard/technical-task-simple-user-management-crud)

A Laravel 12 REST API with a Vue 3 and Inertia admin dashboard, built as a technical task. It shows how I structure a Laravel API: thin controllers, a service layer, a repository behind an interface, Form Requests that return one consistent 422 error shape, and API Resources for the response. API clients get Sanctum bearer tokens; the dashboard uses Breeze session auth for a separate `backend_users` table, with roles and permissions from spatie/laravel-permission. Deleted users are soft-deleted, and re-creating one with the same email restores the record instead of failing the unique check. PHPStan runs at level 8 with Larastan, and a Postman collection is included.

Write-up: [Laravel User Management API project page](https://julynardtago-on.netlify.app/projects/laravel-user-management-api/) and [Building a maintainable Laravel API](https://julynardtago-on.netlify.app/articles/building-a-maintainable-laravel-api/).

### [Livewire application baseline](https://github.com/Julynard/livewire)

A Laravel 12 application on the official Livewire starter kit, set up as a baseline for Livewire work: Livewire 4 with Flux UI, Fortify authentication including two-factor, Pest feature tests for the authentication and settings flows, and GitHub Actions that run the tests and Pint.

### Earlier work, 2020 to 2023

- [Final-Guidance](https://github.com/Julynard/Final-Guidance): the student guidance system I built at Philippine Christian University in Laravel 8 with Jetstream and Livewire, including spreadsheet import with Laravel Excel.
- [auth-api-itexmo](https://github.com/Julynard/auth-api-itexmo) and [front-end-ordering-system](https://github.com/Julynard/front-end-ordering-system): a Laravel 10 and Sanctum API for products, customers and checkout, with a queued order-notification email, plus its separate Vue 3 frontend using Pinia and Vue Router.
- [ordering-system](https://github.com/Julynard/ordering-system): an early Laravel 10 ordering exercise with product listing behind login and a Sanctum-protected endpoint for creating products.

## Engineering principles

- **Start from the business requirement.** I write the design spec and test plan before the code, so the rules of the process are agreed before they're encoded.
- **Keep the architecture maintainable.** Small classes with one job, and names that match the business language.
- **Make application boundaries explicit.** HTTP, validation, business logic, data access and response formatting each live in one place.
- **Validate at the edge.** Every input goes through a Form Request, and errors come back in one predictable shape.
- **Authorize every action.** Permissions belong in policies and gates, not in scattered `if` statements.
- **Use transactions for multi-step writes.** A workflow step either completes or leaves no trace.
- **Test the behaviour that matters.** Feature tests around the flows the business depends on, plus static analysis in CI.
- **Measure before optimizing.** Find the slow query or the N+1 first, then fix it and check again.
- **Document decisions.** READMEs, setup steps and the reasoning behind non-obvious choices.

## Portfolio and profiles

- [Julynard Tago-on's portfolio and resume](https://julynardtago-on.netlify.app/)
- [Projects and public repositories](https://julynardtago-on.netlify.app/projects/)
- [Laravel case studies and engineering notes](https://julynardtago-on.netlify.app/articles/)
- [LinkedIn profile](https://www.linkedin.com/in/julynard-tago-on/)
- [GitHub profile](https://github.com/Julynard)

## GitHub stats

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Julynard&theme=github_dark&bg_color=071512&title_color=79c8b6&text_color=dce9e4&icon_color=4fb7a2&chart_color=4fb7a2" alt="Julynard's GitHub statistics">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Julynard&theme=github_dark&bg_color=071512&title_color=79c8b6&text_color=dce9e4&icon_color=4fb7a2&chart_color=4fb7a2" alt="Julynard's repository languages">

</div>

**Private contributions:** most of my day-to-day commits are in private client repositories. GitHub's contribution graph can count them without exposing repository names or code; the stats cards above use public profile data only.

<img src="./assets/github-footer.svg" alt="Build. Measure. Improve." width="100%">
