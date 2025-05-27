#include <iostream>
#include <vector>
#include <cstdlib>
#include <ctime>

using namespace std;

// Function to get random word from a vector or whatever this thing does,
// someone could probably actually explain it.
string getRandomWord(const vector<string>& wordList) {
    return wordList[rand() % wordList.size()];
}

// Generates tha poetry
string generatePoetryLine() {
    vector<string> articles = {"The", "A"};
    vector<string> adjectives = {"silent", "golden", "lonely", "bright", "dark", "gentle"};
    vector<string> nouns = {"moon", "wind", "bird", "tree", "dream", "star", "storm"};
    vector<string> verbs = {"sings", "whispers", "dances", "falls", "rises", "shines"};
    vector<string> prepositions = {"in", "on", "beneath", "above", "beside", "with"};

    string line;
    line += getRandomWord(articles) + " ";
    line += getRandomWord(adjectives) + " ";
    line += getRandomWord(nouns) + " ";
    line += getRandomWord(verbs) + " ";
    line += getRandomWord(prepositions) + " ";
    line += getRandomWord(articles) + " ";
    line += getRandomWord(nouns);

    return line;
}

int main() {
    srand(static_cast<unsigned int>(time(0))); // Seed random number generator

    int numLines;
    cout << "How many lines of poetry would you like to generate? ";
    cin >> numLines;

    cout << "\nGenerated Poetry:\n" << endl;
    for (int i = 0; i < numLines; ++i) {
        cout << generatePoetryLine() << endl;
    }

    return 0;
}
