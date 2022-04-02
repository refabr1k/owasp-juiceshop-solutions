## Error Handling
### Challenge: Provoke an error that is neither very gracefully nor consistently handled.

After doing [Level 1: Confidential Document challenge](/level%201/confidential-doc.md) navigate to `quarantine` folder and click any of the files, but add some invalid characters such as `'` which will bring you to an unhandled error.

_Note: The error message reveals a number of things: technology/software used, error trace stacks, absolute path of affected file/code including line number. All which could have been prevented by proper error handling by the developer eg. giving a more generic error message._