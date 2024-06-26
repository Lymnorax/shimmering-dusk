#include <iostream>
#include <cstdlib>
#include <ctime>

int main() {
    // Seed the random number generator with the current time
    std::srand(std::time(nullptr));

    std::cout << "Random numbers between 0 and 99:\n";
    for (int i = 0; i < 10; ++i) {
        // Generate a random number between 0 and 9999
        int randomNum = std::rand() % 100;
        std::cout << randomNum << " ";
    }

    std::cout << std::endl;
    return 0;
}
