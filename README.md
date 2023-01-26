<h1>H2 Goat </h2>
<h2>x) read and summarize</h2>

<h3>Security Misconfiguration</h3>
Vulnerabilities include:

- Unnecessary features are enabled or installed
- Default accounts are still enabled
- Errors give out too much information to user
- Latest security features are not used correctly

Prevention examples:

- Minimize unnecessary features, components, docs etc.
- Automate a process for verifying settings and configurations effectiveness
- Automate a repeatable hardening process
- Segment application architecture

<h4>Source</h4>
https://owasp.org/Top10/A05_2021-Security_Misconfiguration/

<h3>Vulnerable and Outdated Components</h3>

Vulnerabilities include:

- Component versions are unknown
- Outdated, unsupported or otherwise vulnerable software (components, libraries, apps etc.)
- Scans are not done regularly to find vulnerabilities

Prevention examples:

- Remove everything that’s unused (dependencies, components etc.)
- Keep and update inventory of both server- and client-side components
- Use only reliable and secured sources for components

<h4>Source</h4>

https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/

<h3>Injection</h3>

Vulnerabilities include:

- Unproper user
- Supplied data handling (not validated etc.)

Prevention examples:

- Prefer to use a safe API
- Utilize positive server-side input validation
- Use SQL controls that prevent mass disclosure of records, like for example LIMIT

<h4>Source</h4>
https://owasp.org/Top10/A03_2021-Injection/

<h2>a) Sequel. Solve SQLZoo:</h2>
<h3>0 SELECT basics</h3>
1.

![0: basics task 1](SQL_ZOO_0_1.PNG)
changed ` WHERE name= 'Germany`

2.

![0: basics task 2](SQL_ZOO_0_2.PNG)


