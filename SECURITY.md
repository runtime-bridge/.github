# Security

## Reporting a problem

Please use GitHub's private vulnerability reporting on the affected repository ("Security" tab, "Report a vulnerability"). Do not open a public issue for security problems. You will get an answer within a week.

## Scope

rbridge starts agent runtimes on your machine and stands between them and the software that gives them tasks. It never reads, stores or forwards provider credentials, starts runtimes with an allowlisted environment, applies a policy profile to permission requests, and stops the whole runtime process tree when a task ends. It is not a sandbox. The threat model in the main repository describes what is and is not protected: <https://github.com/runtime-bridge/rbridge/blob/main/docs/threat-model.md>.

Reports we especially want: anything that lets a runtime or a skill read credentials through rbridge, escape the workspace through rbridge's file or terminal services, bypass a policy denial, or reach another client's sessions in the daemon.
