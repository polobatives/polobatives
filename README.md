👋 Hi, I’m a digital explorer</strong></summary>

👀 Creating digital worlds using code and imagination. 🌌🖥️
🌱 I love experimenting with new technologies and bringing imaginative concepts to life.
💞️ I’m interested in collaborating on projects that push the boundaries of digital creativity.
</details>

Sample Repository: Simple Unity Game with C#

```csharp
using UnityEngine;

public class PlayerController : MonoBehaviour
{
    public float speed = 5.0f;

    void Update()
    {
        float horizontalInput = Input.GetAxis("Horizontal");
        float verticalInput = Input.GetAxis("Vertical");
        Vector3 movement = new Vector3(horizontalInput, 0, verticalInput) * speed * Time.deltaTime;
        transform.Translate(movement);
    }
}
