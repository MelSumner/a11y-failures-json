# Accessibility Failures

This is a JSON file that attempts to itemize all of the ways that websites, web-based applications, and tooling for developers of web-based applications could fail known accessibility criteria. 

## Technical Details

For each itemized criteria, the following information is provided: 

* id (auto incremented number)
* criteria (array)
* description
* help (advice on how to fix the issue described)
* severity
* tags (array)
* testing (array) 

### References used 

* [WCAG 2.1](https://www.w3.org/TR/WCAG21/)
* [ARIA Role documentation](https://www.w3.org/WAI/PF/aria/roles)
* [WCAG Techniques](https://www.w3.org/WAI/WCAG21/Techniques/#techniques)
* [EN 301 549](https://www.etsi.org/deliver/etsi_en/301500_301599/301549/02.01.02_60/en_301549v020102p.pdf)
* [Section 508](https://www.access-board.gov/guidelines-and-standards/communications-and-it/about-the-ict-refresh/final-rule/single-file-version)
* [axe-core](https://github.com/dequelabs/axe-core/tree/develop/lib/rules) (has several "best practices" outlined)

### Severity levels

* Blocker - Complete loss of service, critical functionality, or data with no acceptable workaround. Includes significant privacy and security risks
* Critical - Severe degradation of critical functionality or data; functionality is still available but is severely limited.  No acceptable workaround is available, but use is still possible in a restricted fashion
* Major - Loss of critical functionality or data, but there is a reasonable workaround available
* Minor - Loss or degradation of non-critical functionality or data.  A workaround may or may not be available

### Testing

For each failure item, it should be determined how the item can be tested. Options are:

1. it can be linted for
2. it has/can have an automated test
3. a developer must write the test
4. it must be manually tested for

## Contributing to this repository

Contributions are welcome. To contribute, please follow these steps: 

1. file an issue on the repository that outlines the missing itemization and links to the relevant success criteria.
2. submit a PR that addresses that issue (and only that issue)

Polite language is expected.
