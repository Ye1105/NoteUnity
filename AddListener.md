```
private Button button

private void Awake() //加载脚本实例时调用 Awake
{
    button=GetComponent<Button>();
    button.onClick.AddListener(StartGame);
}

private void StartGame()
{
    ...
}
```