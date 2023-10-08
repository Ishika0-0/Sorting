#include <iostream>
#include <vector>
#include <algorithm>
#include <random>

// Function to check if a vector is sorted
bool isSorted(const std::vector<int>& arr) {
    for (size_t i = 1; i < arr.size(); ++i) {
        if (arr[i] < arr[i - 1]) {
            return false;
        }
    }
    return true;
}

// Function to perform BogoSort
void bogoSort(std::vector<int>& arr) {
    while (!isSorted(arr)) {
        std::random_shuffle(arr.begin(), arr.end());
    }
}

int main() {
    std::vector<int> data = {5, 2, 9, 1, 5, 6};
    
    std::cout << "Unsorted array: ";
    for (int num : data) {
        std::cout << num << " ";
    }
    std::cout << std::endl;
    
    bogoSort(data);

    std::cout << "Sorted array: ";
    for (int num : data) {
        std::cout << num << " ";
    }
    std::cout << std::endl;

    return 0;
}
