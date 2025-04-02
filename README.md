# hello-world1
  def sum_array(nums):
    n = len(nums)
    output = [1]*n
    left_sum = 1
    for i in range(n):
        output[i] = left_sum
        left_sum *= nums[i]
    right_sum = 1
    for i in range(n-1,-1,-1):
        output[i] *= right_sum
        right_sum = nums[i]
        return output
