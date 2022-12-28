# Repro for React Navigation

This has been cloned from the react navigation repo. I've only added an `alert()` for `getPathFromState` in https://github.com/jparkrr/react-navigation-bug/commit/4f19c8485504bf57a08e5e1c2a39bbce1bef92a9

To install and run:
- Clone the repository and run `yarn` in the project root
- Run `yarn example web`

To repro the bug on web:
- Visit http://localhost:19006/link-component/article/gandalf
- Click the blue "GO TO /LINK-COMPONENT/MUSIC" button.
  - The other links don't exhibit the same bug.
- Notice that there is no getPathFromState alert, whereas all other navigations cause it.
