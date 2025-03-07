<h1 align="center">ChessBot</h1>
A chess AI that uses chess.js for move generation and chessboard.js for visualization. Implements Minimax with Alpha-Beta pruning for efficient decision-making. The evaluation function considers material and piece positioning to improve gameplay. Optimized for better strategic moves while maintaining performance.

## Execution Guide:
Open the terminal and run the following commands:
1. Clone the repository:
   ```
   git clone https://github.com/kr1shnasomani/ChessBot.git
   ```

2. Navigate to the project directory:
   ```
   cd ChessBot
   ```

3. Install npm:
   ```
   npm install
   ```
   If already installed, check the version:
   ```
   npm --version
   ```

4. Start the development server:
   ```
   npm start
   ```

5. The code will display two local host links:
   ```
   http://127.0.0.1:8080
   ```
   ```
   http://192.168.16.194:8080
   ```
   Open any one of the links in the browser

6. This is how the project will look like upon successfuly execution:
   
   <img width="1440" alt="image" src="https://github.com/user-attachments/assets/c97cd655-2d9c-44d8-b265-b8fc57d0d754" />

## Repository Structure:
The following is the repository structure:
```
ChessBot/
│── img/
│   └── chesspieces/
│       └── wikipedia/
│           ├── bB.png
│           ├── bK.png
│           ├── bN.png
│           ├── bP.png
│           ├── bQ.png
│           ├── bR.png
│           ├── wB.png
│           ├── wK.png
│           ├── wN.png
│           ├── wP.png
│           ├── wQ.png
│           ├── wR.png
│── lib/
│   ├── chessboardjs/
│   │   ├── css/
│   │   │   ├── chessboard-0.3.0.css
│   │   │   ├── chessboard-0.3.0.min.css
│   │   ├── js/
│   │   │   ├── chess.js
│   │   │   ├── chessboard-0.3.0.js
│   │   │   ├── chessboard-0.3.0.min.js
│   │   ├── LICENSE.txt
│   ├── jquery/
│   │   ├── jquery-3.2.1.min.js
│── js/
│   ├── chess.js
│── .gitignore
│── LICENSE
│── README.md
│── index.html
│── package.json
│── script.js
│── style.css      
```
