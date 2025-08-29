**Jest** is a **JavaScript testing framework** created by Facebook, designed to make writing and running tests for your code **fast, simple, and reliable**.  

---

## 📝 What Jest Is
- **Type:** Open‑source testing framework
- **Primary Use:** Unit testing, integration testing, and snapshot testing
- **Languages/Frameworks:** Works with JavaScript, TypeScript, Node.js, React, Angular, Vue, and more.
- **Philosophy:** “Delightful JavaScript Testing” — minimal setup, rich features, and quick feedback.

---

## ⚙️ Key Features
| Feature | What It Does | Why It’s Useful |
|---------|--------------|-----------------|
| **Zero Config** | Works out‑of‑the‑box for most JS projects | Saves setup time |
| **Snapshot Testing** | Captures a “snapshot” of UI output and compares it in future runs | Detects unintended UI changes |
| **Isolated Tests** | Runs tests in parallel in separate processes | Faster execution, avoids shared state issues |
| **Built‑in Mocking** | Easily mock functions, modules, or timers | Test components in isolation |
| **Code Coverage** | Generates reports showing which code is tested | Helps improve test completeness |
| **Async Testing Support** | Handles promises, async/await, and callbacks | Great for API and DB tests |

---

## 🔍 Example
```javascript
// sum.js
function sum(a, b) {
  return a + b;
}
module.exports = sum;

// sum.test.js
const sum = require('./sum');

test('adds 2 + 3 to equal 5', () => {
  expect(sum(2, 3)).toBe(5);
});
```
Run:
```bash
npx jest
```
✅ Output: Test passes if `sum(2, 3)` returns `5`.

---

## 🚀 Why It’s Popular
- **All‑in‑one:** Includes test runner, assertion library, mocking, and coverage tools — no need to install multiple packages.
- **Speed:** Runs only changed tests by default.
- **Integration:** Works seamlessly with React (but not limited to it).
- **Community:** Widely adopted, well‑maintained, and supported by the OpenJS Foundation.

---

💡 **In your e‑commerce project**:  
You can use Jest to test:
- API endpoints (backend)
- Utility functions (e.g., cart total calculation)
- React components (frontend)
- Database queries (with mocks)

---

I╭─dakash@dakshs-MacBook-Air ~/quickcart ‹main●› 
╰─$ npx create-nx-workspace@latest .


 NX   Let's create a new workspace [https://nx.dev/getting-started/intro]


 NX   Invalid workspace name

The workspace name "." is invalid.
Workspace names must start with a letter.
Examples of valid names: myapp, MyApp, my-app, my_app

╭─dakash@dakshs-MacBook-Air ~/quickcart ‹main●› 
╰─$ npx create-nx-workspace@latest quickcart --directory=.                         1 ↵


 NX   Let's create a new workspace [https://nx.dev/getting-started/intro]

✔ Which stack do you want to use? · node
✔ What framework should be used? · express
✔ Application name · auth-service
✔ Would you like to generate a Dockerfile? [https://docs.docker.com/] · Yes
? Which unit test runner would you like to use? … 
Jest   [ https://jestjs.io/ ]* and give you **ready‑to‑use test cases** so you can talk about them in your interview like you wrote them yourself. Would you like me to prepare that?


ash@dakshs-MacBook-Air ~/quickcart ‹main●› 
╰─$  npx create-nx-workspace@latest quickcart --directory=.

 NX   Let's create a new workspace [https://nx.dev/getting-started/intro]

✔ Which stack do you want to use? · node
✔ What framework should be used? · express
✔ Application name · auth-service
✔ Would you like to generate a Dockerfile? [https://docs.docker.com/] · Yes
✔ Which unit test runner would you like to use? · jest
✔ Would you like to use ESLint? · No
✔ Would you like to use Prettier for code formatting? · No
✔ Which CI provider would you like to use? · github

 NX   Creating your v21.4.1 workspace.

⠹ Installing dependencies with npm
