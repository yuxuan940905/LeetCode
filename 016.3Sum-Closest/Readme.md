###016. 3Sum-Closet  
在确定了第一个元素之后，第2、3个元素的指针该如何设计变动呢？
```cpp
while (left<right)
{
  if (abs(nums[left]+nums[right]-sum)<CurSum)
    更新最小结果;
  if (nums[left]+nums[right]<sum)
     left++;
  else
     right--;
}
```