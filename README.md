## LottoService.cs
```
public class LottoService
{
    public HashSet<int> GetLotto()
    {
        Random rand = new((int)DateTime.Now.Ticks);
        HashSet<int> lottoData = new HashSet<int>(6);

        while (lottoData.Count < 6)
        {
            lottoData.Add(rand.Next(1, 45));
        }

        return lottoData;
    }
}
```
