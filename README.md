## oneshot

A single-fire HTTP server.

### Synopsis

Start an HTTP server which will only serve files once.
If no file is given, oneshot will instead serve from stdin.
If serving from stdin, oneshot will hold the clients connection until receiving the EOF character

```
oneshot [flags]... [file]
```

### Options

```
  -e, --ext string         Extension of file presented to client.
                           If not set, either no extension or the extension of the file will be used, depending on if a file was given.
  -h, --help               help for oneshot
  -m, --mime string        MIME type of file presented to client.
                           If not set, either no MIME type or the mime/type of the file will be user, depending on of a file was given.
  -n, --name string        Name of file presented to client.
                           If not set, either a random name or the name of the file will be used, depending on if a file was given.
  -p, --port string        Port to bind to. (default "8080")
  -q, --quiet              Don't show info messages.
                           Use -Q instead to suppress error messages as well.
  -Q, --silent             Don't show info and error messages.
                           Use -q instead to suppress info messages only.
  -t, --timeout duration   How long to wait for client.
                           A value of zero will set the timeout to the max possible value.
```

###### Auto generated by spf13/cobra on 11-Jun-2020