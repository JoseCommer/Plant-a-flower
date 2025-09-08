class Solution {
public:
    bool canPlaceFlowers(vector<int>& flowerbed, int n) {
        int size = flowerbed.size();
        
        for (int i = 0; i < size; ++i) {
            if (flowerbed[i] == 0) {
                bool empty_left = (i == 0 || flowerbed[i - 1] == 0);
                bool empty_right = (i == size - 1 || flowerbed[i + 1] == 0);
                
                if (empty_left && empty_right) {
                    flowerbed[i] = 1; // Plant a flower
                    --n; // Decrease required count
                    if (n == 0) return true;
                }
            }
        }
        
        return n <= 0;
    }
};
