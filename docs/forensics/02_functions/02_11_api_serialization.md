## src/APIRest.cs

### `APIRest(Root root)` (L20-L33)
- **Does:** Initializes the HTTP listener and binds it to the configured REST URL.
- **Params:** `root: Root`.
- **Returns:** Constructor.

### `Close()` (L35-L38)
- **Does:** Closes the HTTP listener.
- **Params:** None.
- **Returns:** `void`.

### `ChangeAddress(string addr)` (L41-L58)
- **Does:** Updates the HTTP listener prefix and restarts the server.
- **Params:** `addr: string`.
- **Returns:** `bool`.

### `GetAddress()` (L60-L63)
- **Does:** Returns the current listener prefix.
- **Params:** None.
- **Returns:** `string`.

### `IsListening()` (L65-L75)
- **Does:** Reports whether the HTTP listener is active.
- **Params:** None.
- **Returns:** `bool`.

### `Start()` (L77-L95)
- **Does:** Starts the HTTP listener and launches the request handler task.
- **Params:** None.
- **Returns:** `bool`.

### `Stop()` (L97-L110)
- **Does:** Stops the HTTP listener and waits for the handler task.
- **Params:** None.
- **Returns:** `bool`.

### `HandleIncomingConnections()` (L112-L1090)
- **Does:** Asynchronously handles incoming HTTP requests and maps REST commands to Root actions.
- **Params:** None.
- **Returns:** `Task`.

## src/TinyJson.cs (JSONParser)

### `FromJson<T>(this string json)` (L38-L64)
- **Does:** Parses JSON into a typed object using the minimal parser.
- **Params:** `json: string`.
- **Returns:** `T`.

### `AppendUntilStringEnd(bool appendEscapeCharacter, int startIdx, string json)` (L66-L87)
- **Does:** Appends string contents while respecting escape sequences.
- **Params:** `appendEscapeCharacter: bool`, `startIdx: int`, `json: string`.
- **Returns:** `int` — end index.

### `Split(string json)` (L90-L130)
- **Does:** Splits JSON object/array values into token list.
- **Params:** `json: string`.
- **Returns:** `List<string>`.

### `ParseValue(Type type, string json)` (L132-L266)
- **Does:** Parses JSON into a value of the target type (primitive, array, list, or object).
- **Params:** `type: Type`, `json: string`.
- **Returns:** `object`.

### `ParseAnonymousValue(string json)` (L268-L316)
- **Does:** Parses JSON into a Dictionary/List/object without a known type.
- **Params:** `json: string`.
- **Returns:** `object`.

### `ParseObject(Type type, string json)` (L341-L379)
- **Does:** Maps JSON fields into a typed object using reflection.
- **Params:** `type: Type`, `json: string`.
- **Returns:** `object`.
