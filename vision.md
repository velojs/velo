# The Velo Vision

Simple, fast, and tiny.

```ts
import { Velo } from "velo";

const v = new Velo();

app.get("/", () => "hey");

app.get("/json", () => {
	msg: "how r u";
});

app.post("/todo", (v) => {
	const { task } = v.body();
	// ...
	return {
		success: "true",
		data: {
			task,
		},
	};
});

export default app;
```
