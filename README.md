# tareacc2
//implementacion de insert
#include <iostream>
#include <vector>

int main() {
    std::vector<int> v{1, 2, 3, 4, 5};

    int value = 6;
    int* ptr = &value;

    v.insert(v.begin() + 2, *ptr);

    for (auto x : v) {
        std::cout << x << " ";
    }

    return 0;
}
//implementacion de remove
#include <iostream>
#include <vector>

int main() {
    std::vector<int> v{1, 2, 3, 4, 5};

    int* ptr = &v[2];

    v.erase(ptr);

    for (auto x : v) {
        std::cout << x << " ";
    }

    return 0;
}
//implentacion de push_back
#include <iostream>
#include <vector>

int main() {
    std::vector<int> v{1, 2, 3, 4, 5};

    int value = 6;
    int* ptr = &value;

    v.push_back(*ptr);

    for (auto x : v) {
        std::cout << x << " ";
    }

    return 0;
}
