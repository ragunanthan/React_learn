```jsx 
// this is function component
function App() {
  const [count, setCount] = useState(0);

  return (
    <div className="App">
      <p>this is function component</p>
      <button
        onClick={() => {
          setCount(count + 1);
        }}
      >
        click {count}
      </button>
    </div>
  );
}

// this is class component
class Re extends Component {
  state = {
    count: 0,
  };

  render() {
    return (
      <div className="App">
        <p>this is class component</p>
        <button
          onClick={() => {
            this.setState({
              count: this.state.count + 1,
            });
          }}
        >
          click {this.state.count}
        </button>
      </div>
    );
  }
}

```