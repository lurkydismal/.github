# Security Policy

## Supported Versions

I commit to publishing security updates for the latest version of each repository's `main` branch.

## Expectations

I treat security reports equivalent to a P0 priority level. This means that I attempt to fix them as quickly as possible.
I will release a beta or hot fix for any major security report found in the most recent stable version of the program. 

## Reporting a Vulnerability

I use GitHub's security advisory feature to track open security reports. You should expect
a close collaboration as I work to resolve the security vulnerability you have reported. Please reach out to
[lurkydismal@duck.com](mailto:lurkydismal@duck.com) again if you do not receive prompt attention and regular updates.

## Flagging Existing Issues as Security-related

If you believe that an existing GitHub issue is security-related, I ask that you send an 
e-mail to [lurkydismal@duck.com](mailto:lurkydismal@duck.com). The e-mail should include the GitHub issue ID and a short 
description of why it should be handled according to this security policy.

Security reports are not tracked explicitly in the GitHub issue database.

## Disclosure Process

This section describes the process used by Me when handling vulnerability reports.

Vulnerability reports are received via the [lurkydismal@duck.com](mailto:lurkydismal@duck.com) e-mail alias. When receiving
such an e-mail, I will:

1. Reply to the e-mail acknowledging it's receipt. If the e-mail does not describe
an actual vulnerability, the process will stop here. (Unfortunately, I do receive spam, and well-meaning but ultimately misguided reports that do not represent issues for which this process is appropriate, at this address.)
2. Triage the report to evaluate it's impact and if it is a security vulnerability.
3. I will drive it through the fix and release process.
4. Determine if this security report requires a security advisory.
5. Create a new security advisory if an advisory is required. 
6. Reach out to the reporter to ask them if they would like to be involved and whether they would like to be credited. 
For credit, the GitHub security advisory UI has a field that allows contributors to be credited.

## Receiving security updates

Security advisories will be published through GitHub’s advisory system.
You can watch individual repositories or follow me on GitHub for updates.

All repositories do not have a bug bounty program.

## Priorities

The **P0** label indicates a critically dire issue such as a build break, regression, or failure in existing features that keeps Me from shipping the current build. I look at issues with this label frequently. If you find yourself assigning a **P0** label to an issue, please be sure that there's a positive hand-off between filing and a prospective owner for the issue. **P0** bugs should be rare. Normally there should be zero open **P0** bugs. "The world is on fire."

The **P1** label indicates that the issue deserves immediate attention. "A customer is on fire."

The **P2** label indicates that the issue is about to block from shipping or is an important item of technical debt that I want to fix as soon as possible. These may not be worked on immediately (sometimes some **P3** issues are handled first, e.g. when they are particularly egregious), but are top-of-mind. "A customer is about to be on fire."

The **P3** label indicates high-priority issues that are at the top of the work list. This is the highest priority level a bug can have if it isn't breaking the build. Bugs marked **P3** are generally actively being worked on unless the assignee is dealing with a **P0**-**P2** bug (or another **P3** bug).

The **P4** label indicates issues that I agree are important to work on, but not at the top of the work list. This is the default level for bugs. A bug at this priority level may not be fixed for a long time. Sometimes a bug at this level will first migrate to **P3** before I work on them, but that is not required.

The **P5** label indicates issues I think are valid but not important. This is the default level for new feature requests. I am unlikely to work on such issues unless they form part of a long-term strategic plan (see the Roadmap).

The **P6** label indicates valid issues that are unlikely to ever be worked on. I use "thumbs-up" on these issues to promote them to **P5** or higher based on demand.

## References

- For more information on security advisories, see [the GitHub documentation](https://docs.github.com/en/free-pro-team@latest/github/managing-security-vulnerabilities/managing-security-vulnerabilities-in-your-project).
