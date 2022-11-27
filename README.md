## A custom hook for react: useDebounce

### Demo (Codepen)

--

### Install

```yarn add @ferdotnet/use-debounce```

### How to use it?

```
const App = () => {
    const [query, setQuery] = useState('');
    const qDebounced = useDebounce(query);

    const handleChange = (newValue: string) => {
        setQuery(newValue);
    };
  
    return (
        <input type="text" onChange={handleChange} />
    );
});
```
