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

<h2>Darknet Diaries</h2>

<h2>CVE</h2>

![CVE](CVE.PNG)

I followed the tweet link to the original post on GitHub and there was the following explanation of the injection by user nolan124:

![SQL Injection](SQL_Injection.PNG)

A classic case of not filtering/protecting SQL data, making it possible for someone to inject malignent SQL commands to gather excess information from the source. 

<h4>Source</h4>

https://twitter.com/CVEnew/status/1618605980354224128
https://github.com/siteserver/cms/issues/3490

<h2>a) Sequel. Solve SQLZoo:</h2>
<h3>0 SELECT basics</h3>

0.Introducing the world table of countries

![0: basics task 1](SQL_ZOO_0_1.PNG)
changed ` WHERE name= 'Germany`

2.Scandinavia

![0: basics task 2](SQL_ZOO_0_2.PNG)

changed ` WHERE name IN  ('Denmark', 'Norway', 'Denmark');`

3.Just the right size

![0: basics task 3](SQL_ZOO_0_3.PNG)

changed ` WHERE area BETWEEN 200000 AND 250000`

<h2>2 SELECT from World</h2>

1.

![2: select task 1](SQL_ZOO_2_1.PNG)

Nothing to really change

2.

![2: select task 2](SQL_ZOO_2_2.PNG)

changed `WHERE population > 200000000`

3.

![2: select task 3](SQL_ZOO_2_3.PNG)

changed `WHERE population > 200000000` and added `gdp/population`

4.

![2: select task 4](SQL_ZOO_2_4.PNG)

changed `WHERE continent = 'South America'` and added `population/1000000`

5.

![2: select task 5](SQL_ZOO_2_5.PNG)

changed `WHERE name IN ('France', 'Germany', 'Italy')`

<h2>Bonus tasks</h2>
