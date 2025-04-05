# 🧰 Reusable React Hooks

This package contains a collection of **reusable custom React hooks** that you can drop into any project to streamline your development workflow. These hooks cover common needs like toggling state, handling forms, managing local storage, listening for events, and more.

---

## 📦 Included Hooks

### 1. `useToggle`
Toggle a boolean value. Perfect for toggling modals, dropdowns, and menus.

```js
const [isOpen, toggleIsOpen] = useToggle();
```

---

### 2. `useLocalStorage`
Sync state with local storage so it's persistent across reloads.

```js
const [value, setValue] = useLocalStorage('key', 'default');
```

---

### 3. `useClickOutside`
Trigger a callback when a click occurs outside the specified element.

```js
const ref = useRef();
useClickOutside(ref, () => console.log("Clicked outside!"));
```

---

### 4. `useFetch`
Simplify GET API calls with built-in loading and error states.

```js
const { data, loading, error } = useFetch('/api/data');
```

---

### 5. `useDebounce`
Debounce a value (e.g., search term input) with a configurable delay.

```js
const debouncedSearch = useDebounce(searchValue, 300);
```

---

### 6. `useWindowSize`
Track the browser window size and respond to changes.

```js
const { width, height } = useWindowSize();
```

---

### 7. `useOnlineStatus`
Track whether the user is currently online or offline.

```js
const isOnline = useOnlineStatus();
```

---

### 8. `usePrevious`
Access the previous value of a state or prop.

```js
const prevValue = usePrevious(currentValue);
```

---

### 9. `useForm`
Handle form state with ease. Manage form inputs in a simple way.

```js
const [formValues, handleInputChange] = useForm({ name: '', email: '' });
```

---

## 🛠 Usage

1. Copy the hooks you need into your project.
2. Import and use them in your components.

```js
import useToggle from './hooks/useToggle';
```

---

## 📂 Structure

```
reusable-hooks/
├── useClickOutside.js
├── useDebounce.js
├── useFetch.js
├── useForm.js
├── useLocalStorage.js
├── useOnlineStatus.js
├── usePrevious.js
├── useToggle.js
├── useWindowSize.js
└── README.md
```

---

Enjoy fast, clean, and reusable React development 🚀
