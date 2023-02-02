---
name: Request a new package
about: Ask for a new package to be added to Fedora Silverblue
title: 'New Package Request: <package name>'
labels: 'enhancement'
assignees: ''

---

Please try to answer the following questions about the package you are requesting:

1. Is the package installed by default in Fedora Workstation? If it is not, we will ask you to [open an issue in the issue tracker](https://pagure.io/fedora-workstation/issues) for the [Fedora Workstation Working Group](https://docs.fedoraproject.org/en-US/workstation-working-group/).

2. What, if any, are the additional dependencies on the package? What is the output of this command on a system without overrides or locally installed packages:

```bash
rpm-ostree install --dry-run <package>
```

3. What is the size of the package and its dependencies?

```bash
rpm -qi <package>
```

4. What problem are you trying to solve with this package? Or what functionality does the package provide?

5. Can the software provided by the package be run from a container? Explain why or why not.

6. Can the tool(s) provided by the package be helpful in debugging container runtime issues?

7. Can the tool(s) provided by the package be helpful in debugging networking issues?

8. Is it possible to layer the package locally via `rpm-ostree install <package>`? Explain why or why not.
