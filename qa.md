# Quality Assurance Challengue

The assignment is designed to check your qa and problem-solving skills. We are more interested in test automation, project documentation and testing strategies.

**Purpose:** to test a large, content-focused website like [Páginas Amarillas](https://paginasamarillas.com.do)

**Instructions:** create a test plan for the site, which should include steps to identify both visual and functional defects on multiple browsers, devices, and platforms.

## Pre-QA questions:

- What is the scope and timeline/budget?
  - What features, flows or pages need to be tested?
  - Is there a list of user flows?
  - What browsers (+versions) are in scope?
  - What devices (+versions) are in scope?
- Is this for functional, design and/or accessibility quality assurance?
  - What are the functional requirements?
  - Where are the approved designs?
- What environment is being tested?
- Will I need test accounts, credit cards or other credentials?
- How do developers expect to receive bugs for failures? _e.g. JIRA tickets, verify necessary info_
- Who do bugs get assigned to? _e.g. back to project manager_

# Assumptions

- Performance testing, development QA, stress testing, API testing, etc. are considered for this test plan.
- Using of testing tools or test case management tools like Selenium or Zephyr

# Tasks

- Determine scope
- Create test cases
- Test the site
- Report issues (log bugs)
- Regression testing

## Exploratory QA

- Test for usability
- Check all internal and external links, phone numbers, and spelling
- HTML validation
- Test form validation. Some examples:
  - What is required vs. optional?
  - Can you enter anything in the email address or zip code field?
  - If the application stops you from advancing, is there clear direction?
- Click through all navigation, including breadcrumbs
- Keep visual consistency in mind
  - e.g. look at how buttons and links are styled, compare from page to page or tool to tool
- Test atypical scenarios and for error checking
  - e.g. what happens if you don’t enter a search term and click Search?
- Ask questions like “Is this intuitive?” or “How much do I need to read or remember to move forward?”

## Design QA

- Obtain approved designs
- Proofread all content and check that the language matches the approved copy
- Check for hoverstates, animations, and other dynamic visuals not represented in static designs
- Check for visual consistency between approved designs and web pages on ALL viewport sizes (desktop, tablet, mobile)
- Cross-browser testing
- Validate or create tickets for failures

## Functional QA

- Obtain list of requirements
- Develop test strategies and cases based on requirements + pages/features/flows
- Run test cases
- Mark requirements as resolved or create tickets for failures

## Accessibility QA

- Accessibility or compliance?
- Validate HTML
- Run automated tests
- Attempt all user flows and navigation using
  - only the keyboard
  - screen readers (e.g. JAWS, VoiceOver, NVDA)
- Check for contrast issues, readable font sizes, and consistent & intuitive styling
