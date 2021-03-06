# Accessibility Failures

This is a JSON file that attempts to aggregate and uniformly itemize all of the mechanisms by which websites, web-based applications, and their associated developer tools can lead to failures in achieving known accessibility success criteria. 

Currently, a single data source that contains all of this information does not exist. In principle, the completed dataset provides a much-needed consolidation of web accessibility failure reference information, and could be used for any number of custom applications (to track issues, guide accessibility engineering work, create new tooling, etc).

NOTE: This is currently a work in progress!

## Technical Details

For each itemized criteria, the following information is provided: 

* id (string; auto-incremented number)
* criteria (array; WCAG, EN or Section 508 reference(s))
* description (string; short descriptor of issue)
* help (string; advice on how to fix the issue described)
* severity (string; should be single value of blocker, critical, major or minor (outlined below))
* tags (array; should be logical and consistent with the others)
* testing (array; can have multiple values (outlined below))

### References used 

* [WCAG 2.1](https://www.w3.org/TR/WCAG21/)
* [ARIA Role documentation](https://www.w3.org/WAI/PF/aria/roles)
* [WCAG Techniques](https://www.w3.org/WAI/WCAG21/Techniques/#techniques)
* [EN 301 549](https://www.etsi.org/deliver/etsi_en/301500_301599/301549/02.01.02_60/en_301549v020102p.pdf)
* [Section 508](https://www.access-board.gov/guidelines-and-standards/communications-and-it/about-the-ict-refresh/final-rule/single-file-version)
* [axe-core](https://github.com/dequelabs/axe-core/tree/develop/lib/rules) (has several "best practices" outlined)

### Severity levels

While a page's conformance is a pass or fail, giving itemized failures a severity level can help prioritize work. All issues, no matter what their severity, must be resolved for a page to be conformant.

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
