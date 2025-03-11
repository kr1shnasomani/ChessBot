<h1 align="center">ChessBot</h1>
A chess AI that uses chess.js for move generation and chessboard.js for visualization. Implements Minimax with Alpha-Beta pruning for efficient decision-making. The evaluation function considers material and piece positioning to improve gameplay. Optimized for better strategic moves while maintaining performance.

## Execution Guide:
Run the following commands in the terminal:
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

5. The code will display two local host links, open any of the links in the browser:
   ```
   http://127.0.0.1:8080
   ```
   ```
   http://192.168.16.194:8080
   ```

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
└──style.css      
```

## Code Output:

<div align="center">
  <img src="https://cdn-media-1.freecodecamp.org/images/1*sX_XwfPrOQ6c62iuVZ75fw.gif" alt="GIF">
</div>

## Overview:
### 1. Move Generation & Board Visualization:
We use `chess.js` for move generation and `chessboard.js` for visualization. The move generation library handles chess rules, allowing us to calculate legal moves. Our initial function picks a random move from all possible moves.

<img width="662" alt="image" src="https://github.com/user-attachments/assets/86015b57-374f-4298-8b12-debd998d4269" />

### 2. Position Evaluation:
To evaluate positions, we assign piece values:

<img width="383" alt="image" src="https://github.com/user-attachments/assets/9ed38fee-9c1f-409d-8ce3-21cfc75aebae" />

The algorithm now prioritizes capturing pieces when possible.

### 3. Minimax Algorithm:
Minimax explores all possible moves up to a certain depth and evaluates board positions. It selects the move that maximizes the advantage for the current player while minimizing the opponent’s advantage.

![image](https://github.com/user-attachments/assets/edab3d7f-2b03-423a-8a30-e0e64c94c5b4)

### 4. Alpha-Beta Pruning:
Alpha-beta pruning optimizes Minimax by eliminating unnecessary branches, improving search depth and efficiency without affecting outcomes.

![image](https://github.com/user-attachments/assets/d8a5ce97-3895-40fe-9379-1a41d6e92c48)

### 5. Improved Evaluation Function:
Beyond material value, we enhance evaluation using piece-square tables. Piece positioning influences the score—e.g., knights are stronger in the center.

<img width="643" alt="image" src="https://github.com/user-attachments/assets/6f379370-06f1-4ceb-a649-3e16abb25b2f" />
