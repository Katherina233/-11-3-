# （11）邢成婧玉
using System;
namespace Maticsoft.Model
{
	/// <summary>
	/// llog:实体类(属性说明自动提取数据库字段的描述信息)
	/// </summary>
	[Serializable]
	public partial class llog
	{
		public llog()
		{}
		#region Model
		private string _输入账号;
		private string _输入密码;
		private string _重新输入;
		/// <summary>
		/// 
		/// </summary>
		public string 输入账号
		{
			set{ _输入账号=value;}
			get{return _输入账号;}
		}
		/// <summary>
		/// 
		/// </summary>
		public string 输入密码
		{
			set{ _输入密码=value;}
			get{return _输入密码;}
		}
		/// <summary>
		/// 
		/// </summary>
		public string 重新输入
		{
			set{ _重新输入=value;}
			get{return _重新输入;}
		}
		#endregion Model

	}
}
抽象工厂模式的感想
印象最深的就是接口，抽象工厂模式所提供的是创建相互依赖或者有关系的对象的接口，所以具体类的存在就不那么重要了，运用抽象工厂模式可以更好的概括更多的产品对象，进行泛化，从而可以统一功能中的共性，更好的合理分类，而不是具体成一个产品。比如对于电器它们有共同点，客户可能需要对耗电量进行衡量，小电器之间相互关联依赖形成产业链，，就有牵一发而动全身的改变发生。抽象工厂模式创建的接口，把它们全部封装于类，因为之间有逻辑联系，再开发或者维护的过程中，对这个类的编译就要比每个具体类简单有效多了。
所以说抽象工厂模式并不关系每个具体产品的细节，它的优点是创建封装产品的公共接口，用子类决定创建类。这样既可以在不改变工厂的前提下引进新产品。
