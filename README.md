# DD4T.Model HOTFIXED for Concurrency Issues
### Merged from Branch_2.0.7-CONCURRENCY_HOTFIX
Provides a **HOTFIXED** version of the DD4T.Serialization assembly adapted from DD4T v2.0.7 -- the main version used by most versions of DXA. It contains patched logic ported from 
DD4T v2.2.2 (fixed in [this commit #ff96b15](https://github.com/dd4t/DD4T.Model/commit/ff96b151f06f242989449aa9f84ae7408f358db6)), to address the concurrency/locking issues that yield highly unstable environments for both Content Management and Content Delivery. This is key dependency of 
DXA v1.3-v1.8, all of which suffer from the instability and concurrency issues.

**The problem, resolution, and purpose of this HOTFIX Branch has been documented in much more detail in the Github issue here: https://github.com/dd4t/DD4T.Model/issues/35**

This is intended to help out others that need, or want, quick access to a working HOTFIX version of the DD4T.Serialization assembly.  This, in combination with updating Newtonsoft JSON.Net reference to v10+, will help fix the concurrency issues that plague both the Content Delivery application as well as their Content Management template building blocks that leverage DD4T and are impacted by the issues documented in the above Github issue, and/or cross linked StackOverflow issues, as follows:

1. https://tridion.stackexchange.com/questions/17961/dxa-1-2-intermittent-issue-in-json-output
2. https://tridion.stackexchange.com/questions/18235/dxa-1-5-intermittent-issue-in-json-output

## DD4T content model (.NET)
Contains the model classes used in DD4T templates as well as the DD4T presentation layer for .NET.

### Disclaimer:
THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

