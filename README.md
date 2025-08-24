Step 1: Create a Vite + React Project

    npm create vite@latest makyo-dropdownlist-demo -- --template react
    cd makyo-dropdownlist-demo
    npm install

Step 2: Install the Package

    npm install https://github.com/aethercorp-solutions/makyo-searchable-dropdown-list

Step 3: Update App.jsx (or App.tsx if using TypeScript)

    import { useState } from 'react'
    import './App.css'
    import { MultiSelectDropdown } from 'makyo-searchable-dropdown-list'

    const options = [
        'Option 1',
        'Option with icon',
        'Long Long Option 3',
        'Long Long Long Option 4',
        'Long Long Long Long Option 5',
        'Long Long Long Long Long Option 6'
    ];

    function App() {
        const [count, setCount] = useState(0);

        return (
            <div className="App">
                <h1>Makyo Searchable Dropdown Demo</h1>
                <MultiSelectDropdown 
                    options={options}
                    multiple={true}
                    outlined={false}
                    optionLabel="Label"
                    filtering={true}
                    usePortal={false}
                />
            </div>
        );
    }

 export default App;   

Step 4: Run the App

    npm run dev

Open your browser to http://localhost:5173 (or the URL shown in your terminal).

The deployed url is:

    https://aethercorp-solutions.github.io/makyo-dropdownlist-demo/


