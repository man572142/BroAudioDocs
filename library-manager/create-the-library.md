# Create The Library

When you open the Library Manager,  you will see the two major section of the library creation.

## Drag And Drop or Browse

This is pretty straightforward, you can bring any AudioClip into the library by drag and drop or browse. It will create an Asset and one (or more) Entity automatcially.&#x20;

If multiple AudioClips are dropped. A confirmation window will pop up to ask you how would you like to structure them, these options are:

**1.  Multiple For Each:** Create multiple entities for each audio clip.

**2. One For All:** Create one entity, and adds all the audio clips to the entity's clip list.

當asset被建立時，它會自動被命名為"Temp" (因為是一個.asset檔，理所當然需要一個檔名)，此時你可以開始編輯這個asset，不過如果要能夠在playMode中使用他的話，請記得給他一個正式的名稱。你可以點擊左上方的Temp來更改名稱。



Seem the asset is a scriptable object (a .asset file), it will be named as "Temp", which will require a proper naiming in order to be used at runtime.&#x20;

## Asset List

If you have created any assets before, they will appear in the list. You can access the asset to modify its content by double-clicking it.&#x20;

The asset list works like a ordinary list that shows in the inspector, but with slightly different conseqence with the action as below.

**Add(+):**\
It will create an element and a scriptable object asset, and a naming window will pop up to ask you name the asset.

**Remove(-):**\
It will remove both the element in the list, and the asset file it's refering to.

**Double-clicking an element**\
It will open the asset and its entities collection ready for modification.

