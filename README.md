# Arya-Matics
#include <iostream>
#include <cstdlib>  // For rand() and srand()
#include <ctime>    // For time()

int main() {
    std::srand(std::time(0)); // Seed for random number generation

    int sum = 0;
    std::cout << "Generated Random Numbers: ";

    for (int i = 0; i < 5; i++) {
        int num = std::rand() % 100; // Generates random number between 0 and 99
        std::cout << num << " ";
        sum += num;
    }

    std::cout << "\nSum of the numbers: " << sum << std::endl;

    return 0;
}
