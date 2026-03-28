
📦 1. Fetch API
🔹 What it is

Used to make HTTP requests (GET, POST, etc.) to servers/APIs.

🔹 Basic Syntax
fetch("https://api.example.com/data")
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.log(error));
🔹 Example
fetch("https://jsonplaceholder.typicode.com/posts")
  .then(res => res.json())
  .then(data => {
    console.log(data);
  });

🔁 2. Promises
🔹 What is a Promise?

Represents a value that may be available:

Now
Later
Never (error)
🔹 States
Pending
Resolved
Rejected
🔹 Creating a Promise
let promise = new Promise((resolve, reject) => {
  let success = true;

  if (success) resolve("Done!");
  else reject("Error!");
});
🔹 Using Promises
promise
  .then(result => console.log(result))
  .catch(error => console.log(error));

⏳ 3. Async / Await
🔹 What it is

Cleaner way to handle Promises (looks synchronous)

🔹 Syntax
async function getData() {
  let response = await fetch("https://api.example.com/data");
  let data = await response.json();
  console.log(data);
}
🔹 Example
async function fetchPosts() {
  try {
    let res = await fetch("https://jsonplaceholder.typicode.com/posts");
    let data = await res.json();
    console.log(data);
  } catch (err) {
    console.log(err);
  }
}
fetchPosts();

🔍 Difference: =, ==, ===
1. = (Assignment)

Used to assign value

let x = 5;

👉 “Put 5 into x”

2. == (Loose Equality)

Compares values only (does type conversion)

5 == "5"   // true ✅

👉 JS converts "5" → number → compares

⚠️ This is called type coercion (can cause bugs)

3. === (Strict Equality) ✅ IMPORTANT

Compares:

value ✔️
type ✔️
5 === "5"   // false ❌

👉 number ≠ string → false

🧠 Rule (VERY IMPORTANT)

👉 Always prefer:

=== and !==

❌ Avoid:

== and !=

Because:

== can behave unpredictably