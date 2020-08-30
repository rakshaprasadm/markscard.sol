# markscard.sol


pragma solidity 0.4.16 <= 0.6.12;


contract maskcard{
    string name;
    string class;
    string addre;
    int roll;
    int age;
    int marks;
    
    function maskcard(string newName, string newclass, string newaddre,int newroll, int newage, int newmarks) public {
        name = newName;
        class = newclass;
        addre = newaddre;
        roll = newroll;
        age = newage;
        marks = newmarks;
    }
    
    function getmarkscard() public view returns(string, string, string,int, int, int){
        return(name, class, addre, roll, age, marks);
    }
}
