## A custom hook for react: useDebounce

### Demo (Codepen)

https://codepen.io/ferdotnet/pen/MWXXzbg

### Install

```yarn add @ferdotnet/use-debounce```

### How to use it?

```
const App = () => {
    const [query, setQuery] = useState('');
    const qDebounced = useDebounce(query);
    
    const handleChange = (el) => {
        setQuery(el.target.value);
    };
    
    return (
        <div className="wrapper">
            <input type="text" placeholder="Write something here.." onChange={handleChange} />
            <span>{qDebounced || '👀'}</span>
        </div>
    );
});
```
